---
title: Access Database
navcat: Workflows
tags:
---
## Preparing the data file

1. Pull up the data you want to migrate in the Specimen table of the Access database. Copy the data and paste into Excel. Flag all of the rows in Access as "migrated-to-EMu" by using Find & Replace on the (you can find blank cells by searching for "Null").
1. Save as a CSV, then open the CSV in OpenRefine.
1. Run the script *_OpenRefineScript_AccessSpms-to-EMu.json* in OpenRefine. This will take care of  basic transformations needed to prepare the data for EMu. Make sure that the project value (**IPProject**) is correct for your data! Data in all columns should be verified, with special attention to the following...
  - Deal with any data in the column **locMod**, then delete this column.
  - Deal with any data in the column **Flag**, then delete this column. The value "provisional" in this column should have automatically been converted to a value of "unknown" in the column **IPDisposition**.
  - Deal with any data in the column **Comments**, then delete this column.
  - Verify data in the columns **IPCollection**, **IPTypeNo** and **InvTypeStatus**. All rows that have a type number and status should have a value of "TYPE" for **IPCollection**.
  - Verify data in the columns **IPCatInstCode_tab** (for the institution code, e.g. "UCLA") and **IPCatInstNumber_tab** (for the number, e.g "38469"). If there are multiple numbers, make sure to add an additional column pair for each set, named e.g. **IPCatInstCode_tab(2)** + **IPCatInstNumber_tab(2)**.
  - Convert the dates in **AdmDateInserted** to ISO standard, i.e. YYYY-MM-DD.
1. Review and transform the data for the accepted identification. This has been left un-automated in order to ensure the highest level of data quality control.
  - Check the column **KenNo** for any information. This data is only necessary if both **SpecTaxNo** and **OriginalID** are blank. Delete **KenNo** after checking.
  - Review and fix data in **Ide2IdentifiedBy1_tab(1)**. Replace abbreviations where full names are known, e.g. "LouElla Saul" rather than "L. Saul." All rows should have values; use "unknown" where necessary.
  - Convert the dates in **Ide2DateIdentified0(1)** to ISO standard, i.e. YYYY-MM-DD. Add a year for recent identifiers, e.g. if **Ide2IdentifiedBy1_tab(1)** is "Erica Krimmel" enter "2018" for the value of **Ide2DateIdentified0(1)**.
  - Look up the EMu IRNs for each **SpecTaxNo** value using the snippet `cell.cross("access-taxonomy-crosswalk_2019-01-03","TaxTaxNo").cells["EMUIRN"].value[0]`. You'll need to edit the name of the current taxonomy crosswalk when necessary. Name the new column **Ide2TaxonRef_tab(1).irn**. Make sure that every row has a value in this field.
  - Add a new column based on the XX called **Ide2Qaulifier_tab(1)** using the snippet `cell.cross("emu-taxonomy_2019-01-03","irn").cells["Ide2Qaulifier_tab"].value[0]`.
  - Add a new column based on the XX called **Ide2QualifierRank_tab(1)** using the snippet `cell.cross("emu-taxonomy_2019-01-03","irn").cells["Ide2QualifierRank_tab"].value[0]`.
  - Spot check that this name is valid using the code snippet `cell.cross("emu-taxonomy_2019-01-03","irn").cells["ClaCurrentlyAccepted"].value[0]`.
1. Review and transform the data for the original identification. This has been left un-automated in order to ensure the highest level of data quality control.
  - Look up the EMu IRNs for each **OriginalID** value using the snippet `cell.cross("access-taxonomy-crosswalk_2019-01-03","TAXON").cells["EMUIRN"].value[0]`. You'll need to edit the name of the current taxonomy crosswalk when necessary. Name the new column **Ide2TaxonRef_tab(2).irn**. You can also try looking up irns in the *emu-taxonomy* file. Inevitably, you will need to look up some names by hand. Every row in this column needs a value. May need to create names in EMu.
  - Once you have EMu irns for each row where **OriginalID** has a value, delete the **OriginalID** column and add the following columns based on **Ide2TaxonRef_tab(2).irn** by looking up values from the *emu-taxonomy* file: **Ide2Qaulifier_tab(2)**, **Ide2QualifierRank_tab(2)**. Add another two columns where you autofill "No": **Ide2FiledAs_tab(2)**, **Ide2CurrentID_tab(2)**.
  - If necessary, use the column **Ide2Comments0(2)** to record notes about an identification, or to record a name that is not appropriate to add to the EMu taxonomic dictionary.
1. Add collector and date information
1. Export two versions of CSV from OpenRefine, one excluding the column "SpecIRN." Save the version with this column to the Dropbox folder *EMu --> Data Migration Archive --> Catalogue* and use the version without this column to load into EMu.

## Migrating data into EMu

1.
