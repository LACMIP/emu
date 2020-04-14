---
title: Migrating (Access)
navcat: Workflows
tags:
last_modified_at: 2020-04-14 [archived]
---
LACMIP was cataloging specimens in Microsoft Access from 2015 to July 2019; however, cataloging now occurs in EMu. The process to migrate data from Access into EMu is archived here. This page is no longer updated.

## Extract from Access

1. Pull up the data you want to migrate in the Specimen table of the Access database. Copy the data and paste into Excel, then save as a CSV.
1. In the Access column *MigrationStatus* flag all of the rows you just copied with the value "yes" by using Find & Replace (you can find blank cells by searching for "Null").
1. Import the newly-saved CSV into OpenRefine.

## Verify basic data

**Run the script *[_OpenRefineScript_AccessSpms-to-EMu.json]({{ site.url_scripts }})*** in OpenRefine. This will take care of basic transformations needed to prepare the data for EMu. Data in all columns should be spot-checked to verify, with special attention to the following...

1. Deal with any data in the column *locMod*, then delete this column.
1. Make sure that the project value (*IPProject*) is correct for your data; the default value is currently set to "EPICC."
1. Deal with any data in the column *Flag*, then delete this column. The value "provisional" in this column should have automatically been converted to a value of "unknown" in the column *IPDisposition*.
1. Deal with any data in the column *Comments*, then delete this column. Or if there are comments that need to remain with the record, retain them in a column named *InvLotRemarks*.
1. Check data in the columns *IPCollection*, *IPTypeNo* and *InvTypeStatus*. All rows that have a type number and status should have a value of "TYPE" for *IPCollection*.
1. Check data in the columns *IPCatInstCode_tab* (for the institution code, e.g. "UCLA") and *IPCatInstNumber_tab* (for the number, e.g "38469"). If there are multiple numbers, make sure to add the suffix "(1)" after the first two column names and add an additional column pair for each set, named e.g. *IPCatInstCode_tab(2)* + *IPCatInstNumber_tab(2)*.
1. Convert the dates in *AdmDateInserted* to ISO standard, i.e. YYYY-MM-DD.

## Verify taxonomic identification data

**Review and transform data related to the ACCEPTED identification.** This has been left un-automated in order to ensure the highest level of data quality control...

1. Check the column *KenNo* for any information. This data is only necessary if both *SpecTaxNo* and *OriginalID* are blank. Delete *KenNo* after checking.
1. Review and fix data in *Ide2IdentifiedBy1_tab(1)*. Replace abbreviations where full names are known, e.g. "LouElla Saul" rather than "L. Saul." All rows should have values; use "unknown" where necessary.
1. Convert the dates in *Ide2DateIdentified0(1)* to ISO standard, i.e. YYYY-MM-DD. Add a year for recent identifiers, e.g. if *Ide2IdentifiedBy1_tab(1)* is "Erica Krimmel" enter "2018" for the value of *Ide2DateIdentified0(1)*.
1. Look up the EMu IRNs for each *SpecTaxNo* value using the "Add column based on this column" command with code snippet `cell.cross("access-taxonomy-crosswalk_2019-01-03","TaxTaxNo").cells["EMUIRN"].value[0]`. Name the new column *Ide2TaxonRef_tab(1).irn*, and make sure that every row has a value.

    In this and each subsequent step that uses the `cell.cross` command, you'll need to have the [current crosswalk]({{ site.url_lookups }}) (e.g. *access-taxonomy-crosswalk_2019-01-03*) loaded into your instance of OpenRefine, and you'll also need to edit the name of the crosswalk in the code snippet if it differs.
    {: .notice--warning}

1. **Once you have an EMu IRN for every row**, delete the *SpecTaxNo* column and add a new column based on *Ide2TaxonRef_tab(1).irn* called *Ide2Qaulifier_tab(1)* using the snippet `cell.cross("emu-taxonomy_2019-01-03","irn").cells["Ide2Qaulifier_tab"].value[0]`.
1. Add a new column based on *Ide2TaxonRef_tab(1).irn* called *Ide2QualifierRank_tab(1)* using the snippet `cell.cross("emu-taxonomy_2019-01-03","irn").cells["Ide2QualifierRank_tab"].value[0]`.
1. Check that the names in Access are still up-to-date by adding a new column based on *Ide2TaxonRef_tab(1).irn* using the snippet `cell.cross("emu-taxonomy_2019-01-03","irn").cells["ClaCurrentlyAccepted"].value[0]`. Delete this column after you look for, and resolve, any rows with a value of "No."

**Review and transform the data related to the ORIGINAL identification.** This has been left un-automated in order to ensure the highest level of data quality control...

1. Look up the EMu IRNs for each *OriginalID* value using the "Add column based on this column" command with code snippet `cell.cross("access-taxonomy-crosswalk_2019-01-03","TAXON").cells["EMUIRN"].value[0]`. Name the new column *Ide2TaxonRef_tab(2).irn*. **Each existing value for *OriginalID* needs to be either converted to a value for *Ide2TaxonRef_tab(2).irn* or recorded as a comment in *Ide2Comments0(2)***. Inevitably, you will need to look up some names by hand, and you may need to create names in EMu for taxonomy that is invalid but still a concept we want to track (see [Taxonomy Module documentation]({{ site.baseurl }}/documentation/taxonomy/) for more on this).
1. Once you have EMu IRNs for each row where *OriginalID* has a value, delete the *OriginalID* column and add the following columns based on *Ide2TaxonRef_tab(2).irn* by looking up values from the *emu-taxonomy* crosswalk (as described in the accepted identification steps above): *Ide2Qaulifier_tab(2)*, *Ide2QualifierRank_tab(2)*.
1. Add another two columns where you autofill "No" for any row with a value in the  *Ide2TaxonRef_tab(2).irn* column: *Ide2FiledAs_tab(2)*, *Ide2CurrentID_tab(2)*.
1. If necessary, use the column *Ide2Comments0(2)* to record notes about an identification, or to record a name that is not appropriate to add to the EMu taxonomic dictionary.

## Add collecting event data

1. Add **collector information** for each *SitSiteRef_tab.SitSiteNumber* by using the "Add column based on this column" command with code snippet `cell.cross("locality-collector-and-date_2019-01-16", "SitSiteNumber").cells["IPCollName_tab"].value[0]`.
1. Add **collecting start date information** for each *SitSiteRef_tab.SitSiteNumber* by using the "Add column based on this column" command with code snippet `cell.cross("locality-collector-and-date_2019-01-16", "SitSiteNumber").cells["IPStartDate0"].value[0]`.
1. Add **collecting end date information** for each *SitSiteRef_tab.SitSiteNumber* by using the "Add column based on this column" command with code snippet `cell.cross("locality-collector-and-date_2019-01-16", "SitSiteNumber").cells["IPEndDate0"].value[0]`.

## Load into EMu

1. **Export a CSV from OpenRefine** to load into EMu, and save a copy to the folder *Dropbox > EMu > Data Migration Archive > Catalogue*.
1. If you are accessing EMu via the VPN, drag and drop the CSV file into the remote desktop and open the file from within the remote desktop. For whatever reason, opening the file helps EMu recognize it as a valid format.
1. Open the Catalogue module of EMu and follow the instructions for a [custom import]({{ site.baseurl }}/documentation/import/). Remember that validating your file *before* importing it is a good way to double-check your work and avoid headaches later.
