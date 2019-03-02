---
title: Taxonomy
navcat: Modules
tags: quick-start taxonomy
last_modified_at: 2019-03-01
---
The Taxonomy module is the primary record for information about taxonomic concepts, both accepted and unaccepted. Please see [Axiell's documentation](http://help.emu.axiell.com/latest/en/Topics/EMu/Taxonomy%20module.htm) for generic information about this module.

## Taxonomic hierarchy

Taxonomy in EMu follows familiar hierarchical levels, beginning with kingdom and ending with subspecies. LACMIP taxonomy records only use sub-, super-, and infra- levels where useful. The *Kingdom* field is hidden, but you can see kingdom level records (e.g. Plantae and Animalia) by searching for *Rank* = "kingdom."

EMu stores taxonomy as a massive lookup list. Each level of taxonomic hierarchy, e.g. species or family or subclass, is a level in the lookup list. This means that you can find records based on their relationships to other records, like all the species in a genus. This also helps LACMIP maintain updated taxonomy because edits made to parent records automatically affect child records; for instance, if the name of a genus changes you only need to edit the single genus-level record and all the species within that genus will inherit those changes.

If you need to edit the rank of a taxonomy record, e.g. "Psocodea exists as an order but should now be a superorder," you'll need to contact the Museum's database manager, as LACMIP staff do not have permission to make these edits.

## Creating a new taxonomy record

Prior to creating a new taxonomy record, it is essential that you search for it to make sure your taxon doesn't already exist in EMu. We occasionally have duplicate taxon records where the name is unaccepted and needed to be synonymized with two different valid names, but in no other circumstance should we create duplicate taxonomy records. **EMu will not give any kind of warning if you are about to create a duplicate**, so the responsibility is on you.
{: .notice--warning}

### Invertebrates tab

To create a new taxonomy record, click on the "new" icon in the top toolbar and EMu will bring up a blank record that looks like the figure below.

{% include figure image_path="/assets/images/taxonomy_invertebrates.png" alt="Invertebrates tab of the EMu taxonomy module" caption="Screenshot of the *Invertebrates* tab of the Taxonomy module, with the necessary fields to create a new taxon record (in this example, for a species) highlighted." %}

The initial tab of a taxonomy record contains the core taxonomic concept information. **The first field you need to fill out is the lowest taxonomic rank of the taxon you are creating**, e.g. if you need to create a new record for "Calva varia" you would enter "varia" in the *Species* field, or to create a record for "Inoceramidae" you would enter "Inoceramidae" in the *Family* field. **You will only ever enter data into one level of the taxonomic hierarchy fields.**

**The next field you need to fill out is the *Parent Taxon* field**. This should be the direct parent of your new taxon, e.g. for "Calva varia" the *Parent Taxon* would be the genus "Calva", or for "Inoceramidae" the *Parent Taxon* would be the order "Pteriida." If your parent taxon does not already exist in EMu, you can open up an additional Taxonomy module window to create it and then attach it here.

The other fields on this tab are...

Taxon Code
: Not in use, although in the Taxonomy module search, you can enter a value into this field and EMu will look for it in *all* levels of taxonomic hierarchy (rather than you having to know that, e.g. it is a genus).

Automatic?
: Leave this as "No."

Author String
: Author information for the taxon, formatted as is typical e.g. "Author & Author, Year". Use ampersands (&) rather than "and."

Rank
: EMu will assign the value to this field based on the lowest taxonomic rank of the record, e.g. the taxon "Calva varia" will be assigned the rank "Species."

Currently Accepted?
: Select either "Yes" for taxonomic names that are accepted, "No" for those that aren't, or "Unknown" for rare cases in which we really cannot determine the status of a name (a good rule of thumb is to only use "Unknown" if the name will never get printed on a specimen label). If you select "No" EMu will prompt you to tell it what the *Current Name* should be. If the current name does not yet exist in EMu, you'll need to open up another Taxonomy module window to create it before attaching it to the unaccepted name. Any accepted taxonomy record linked to unaccepted synonyms will list the synonyms on the *All Synonyms* tab.

Current Name
: See *Currently Accepted*, above. If a name is accepted, then EMu will automatically fill out the *Current Name* field.

### Hierarchy tab

Once you have entered the necessary information on this first tab, save the record and click over to the *Hierarchy* tab where you can see how your new taxon is situated in the LACMIP taxonomy. Unfortunately, the *Hierarchy* tab is not perfect and it displays both accepted and unaccepted names without any differentiation.

{% include figure image_path="/assets/images/taxonomy_hierarchy.png" alt="Hierarchy tab of the EMu taxonomy module" caption="Screenshot of the *Hierarchy* tab of the Taxonomy module. The blue text indicates the taxonomic record at hand." %}

### Descriptions tab

Whenever you create a new taxonomy record, you need to add metadata in the *Descriptions* tab that will help us keep track of when to use this name. The *Descriptions* tab is a generic place for paired values, and it is therefore **very** important that you enter information in here carefully so that we don't accidentally have fields for, e.g. both "Type Specimen" and "Type Specimen**s**."

{% include figure image_path="/assets/images/taxonomy_descriptions.png" alt="Descriptions tab of the EMu taxonomy module" caption="Screenshot of the *Descriptions* tab of the Taxonomy module." %}

The following are currently values we use in the *Descriptions* tab:

*Label* | *Description*
--- | ---
Age Range | Enter information about the geologic age in shorthand. Ex: "K(t)", "K(t)-K(s)", "K(t), K(ca)", "K(t)?"
Project | Assign this taxon to a project; or if the taxon belongs to more than one project enter each project in a separate *Label-Description* pair. Current project options are: "Barstow Arthropods", "Cretaceous Pacific Slope", "EPICC", "McKittrick Tar Pits", "Nonmarine", "Quaternary nonmarine arthropods", "Rancho La Brea Tar Pits", "Statz Collection"
Type specimens | Note any type specimens associated with this taxon in the literature, always including the collection prefix. Ex: "LACMIP Type Number: 4277", "UCMP Type Number: 89753, 89754."
Notes | Random notes about the taxonomic record. Make every effort to find a better home (e.g. maybe on the *Citations* or *Validity* tabs) for information you may be tempted to put here.

## Citations tab

The *Citations* tab is where LACMIP tracks information about species occurrences, so that we can use this to help identify specimens based on where they were collected.

{% include figure image_path="/assets/images/taxonomy_citations.png" alt="Citations tab of the EMu taxonomy module" caption="Screenshot of the *Citations* tab of the Taxonomy module, showing details for one citation in the table of citations. LACMIP does not use the table for *Specimen* and *Type Status*." %}

You will likely need to enter information in the *Citations* tab any time you create a new taxonomy record, or if you are referencing a publication and want to make note of the occurrences it states. LACMIP uses the following fields on this tab...

Cited In
: Attach the [bibliography record]({{ site.baseurl }}/documentation/bibliography/) for the publication you are citing here. If it does not exist yet, you can open a new record in the Bibliography module and create it. If you are citing an occurrence based on a collection rather than a publication, those also exist as bibliography records, e.g. "LACMIP Collection" or "UCLA Collection."

Verified By
: Attach the Parties record for yourself.

Date
: Select today's date.

Cited Locality
: LACMIP uses this field to track specific collecting localities where this taxon is known to occur. These should be listed e.g. "CIT 1154" or "LACMIP 363, LACMIP 8099."

Remarks
: The bulk of your comments will go in this field, because it is where we record information about geographic and stratigraphic occurrence. Format this as "**STATE: Formation: Subunit**", repeating all higher levels for each occurrence. Ex: "CALIFORNIA: Ladd Fm: Baker Canyon; CALIFORNIA: Ladd Fm: Holz Shale." Formations and subunits should be formatted in line with lithostratigraphic information in the LACMIP Sites module. See table below for more formatting examples.

  *Citation Remarks* | *Explanation*
  --- | ---
  STATE: Formation: Subunit | Denotes published species occurrence, or species occurrence found in LACMIP Collections. If the latter, "Cited In:" should also be "LACMIP Collection". Separate multiple occurrences for a given citation with semi-colons.
  [STATE: Formation: Subunit][ANTIQUATED] | Denotes antiquated species occurrence.
  [STATE: Formation: Subunit][SPECIMEN NEEDS EXAMINATION] | Denotes highly suspect species occurrence. If the citation for the occurrence is also the LACMIP Collection, add some additional description for searchability, e.g. [PIERCE OCCURRENCE - SPECIMEN NEEDS EXAMINATION]

Primary Citation
: Check "Yes" for the single citation that best represents this taxon. In other words, if a colleague needed to know more information about this taxon, this is the best reference you could refer them to.

### Using ditto with citations

[Ditto](http://help.emu.axiell.com/latest/en/Topics/Common/The%20Ditto%20utility.htm?Highlight=ditto) can be a very helpful tool when working with citations. You may be adding a citation to one species that also is true for another species--with ditto you'll only need to enter the information into EMu once. The other time that ditto is extremely useful is when taxonomy changes and you need to make a record that has citations unaccepted. You can carry these citations forward to the new accepted name using ditto.

To ditto citations:
1. On the taxonomy record that has citations you'd like to ditto, go to *Edit > Ditto > Use Current Record for Ditto*.
1. On the taxonomy record where you want to add the citations, navigate to the *Citations* tab and then go to *Edit > Ditto > Current Tab*. Keep in mind that using ditto this way will **overwrite any existing citations** so it should only be used on an empty *Citations* tab.

## Validity tab

LACMIP uses the *Validity* tab to track more specific information about the status of a name. Often, all we need to know is the value for *Currently Accepted?* on the *Invertebrates* tab, but sometimes older names are more complicated and the *Validity* tab gives us the space to record this complexity. Validity comments should **not** be related to species **occurrences**; this information is tracked in the *Citations* tab. That said, sometimes the validity of a name varies depending on what geologic timeframe it is applied to, and because we do have specimens from a wide range of timeframes you may need to record that variation on this tab.

{% include figure image_path="/assets/images/taxonomy_validity.png" alt="Validity tab of the EMu taxonomy module" caption="Screenshot of the *Validity* tab of the Taxonomy module." %}

The fields on this tab are...

Reason
: Not in use.

Reference
: Attach a [bibliography record]({{ site.baseurl }}/documentation/bibliography/) to support your validity comment. For comments based on notes or specimens in the collection, this can be the "LACMIP Collection" record. Personal communication can be cited here as well.

Comments
: Enter your comments here. **See table below for preferred comments and formatting consistency.**  If you are unsure of what comment to add, do a wildcard search (*Comments* = `\*`) for all current validity comments in use and proceed accordingly. Suggestion: use the Ditto function to maintain consistency when entering the same comments on multiple taxon records.

  *Validity Comments* | *Explanation*
  --- | ---
  Genus changed in Treatise 1996. | Add if rationale for taxonomic update needs documentation.
  Genus should be in quotation marks. | Track special characters (") using standardized validity comments.
  Genus should be followed by question mark. | Track special characters (?) using standardized validity comments.
  Manuscript name. Species should be in quotation marks. | Call out special characters (") required to format manuscript names using standardized validity comments.
  Name found in collection; validity unknown. | Validity of taxon unknown. This is different than documenting an invalid or questionable taxon occurrence (see *Citations: Remarks* above).
  Show name to R. L. Squires. | Begin "expert opinion" comments with "Show name to…"

Comments by
: Attach the [parties record]({{ site.baseurl }}/documentation/parties/) for yourself or whoever is responsible for this comment.

Date commented
: Enter the date for which the comment was created.


## Permissions

All LACMIP users have more limited permissions in the Taxonomy module than in other modules. You cannot, for example, use the Global Replace tool. Please contact the Museum's database manager for assistance doing tasks you don't have permission for, or to discuss giving you additional permissions.
