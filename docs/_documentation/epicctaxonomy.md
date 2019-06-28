---
title: EPICC Taxonomy
navcat: Workflows
tags: taxonomy
last_modified_at: 2019-06-27
---
The EPICC taxonomic dictionary was migrated from Excel into EMu in Spring 2019. Following this migration will be a transition period and the documentation on this page should be updated to reflect evolving decisions made about managing EPICC taxonomy in EMu. For a column-by-column breakdown of how data was migrated, please refer to the crosswalk tab in the file *Dropbox > EMu > Data Migration Archive > Taxonomy > epicc-taxonomic-dictionary > EPICC_Taxonomy Table Master_MIGRATING_2019-04-12.xlsx*.

All names that originated from the EPICC taxonomic dictionary are flagged as such and can be found by searching *Label*="project" and *Description*="epicc" on the *Description* tab of the Taxonomy module.

**Before following the protocol here, please review documentation for the [Taxonomy module]({{ site.baseurl }}/documentation/taxonomy/).**
{: .notice--warning}

## Citations tab

The *Citations* tab records opinions and distribution details associated with a specific source, be that a publication, a person, a collection, or a consolidation of knowledge like the EPICC Taxonomic Dictionary.

The following Excel columns were migrated into the *Citations* tab:
- *Reference*, where the value is retained in the *Cited In* field and for which the entry was also flagged as the primary citation.
- *Validated*, where the value is retained in the *Cited In* field and paired with a standard comment ("taxonomic data entered") in *Remarks*.
- *Fossil Distribution*, where the value was retained in the *Remarks* field and listed as *Cited In* = EPICC Taxonomic Dictionary.
- *Hall (2002) FAD* and *Hall (2002) LAD*, where the values were retained in the *Remarks* field and listed as *Cited In* = Hall 2002.

{% include figure image_path="/assets/images/epicctaxonomy_citations.png" alt="Citations tab of the EMu taxonomy module" caption="Screenshot of the *Citations* tab of the Taxonomy module, showing details for three citation entries that originated in three different Excel columns. The highlighted data is from *Fossil Distribution* and you can see that it is linked to the bibliography record for the EPICC Taxonomy Dictionary. The middle row in the *Citations* table originated in the *Hall (2002) FAD* and *Hall (2002) LAD* columns, and the top row came from what had been listed in the *Reference* column in Excel." %}

## Validity tab

### Name status

EMu has a field called *Currently Accepted?* to track names that should be used versus synonyms. More detailed information about the name status of EPICC taxonomy can be found on the *Validity* tab, where data from the Excel columns *Category* and *Taxonomic Comments* was migrated.

{% include figure image_path="/assets/images/epicctaxonomy_validity.png" alt="Validity tab of the EMu taxonomy module" caption="Screenshot of the *Validity* tab of the Taxonomy module, showing details for data migrated from the *Category* ('Poor') and *Taxonomic Comments* (always prefaced by 'TAXONOMIC COMMENT') fields in Excel." %}

As with other information that was migrated into EMu based on the Excel version of the EPICC taxonomic dictionary, validity rows displaying data from *Category* and *Taxonomic Comments* are linked to the "EPICC Taxonomic Dictionary" [bibliography]({{ site.baseurl }}/documentation/bibliography/) record.

### Taxonomic name history

EPICC taxonomic name history, including Excel data from the *Original* and *Synonyms* columns, was migrated into EMu's *Validity* tab using the logic diagrammed in the figure below.

{% include figure image_path="/assets/images/epicctaxonomy_decisiontree.jpg" alt="diagram of logic used to migrated EPICC taxonomy name history" caption="Diagram of logic used to migrate EPICC taxonomic name history into the *Validity* tab of the Taxonomy module. This same logic should be used to continue entering new information about taxonomic name history into EMu." %}

As an example of the above, for the name *Anadara camuloensis* the Excel column *Original* listed "Arca camuloensis," and the *Synonym* field had:
> *Arca camuloensis* Osmont, 1905 • *Anadara camuloensis* (Osmont), Woodring, 1938, p. 29, pl. 6, figs. 10, 13-16; Winterer & Durham, 1962, table 4 • *Arca (Larkinia) camuloensis*, *Larkinia camuloensis*  (Osmont) • *Anadara (Larkinia) camuloensis* (Osmont), Durham & Addicott, 1965, table 1 • *Arca (Arca) multicostata camuloensis*

In EMu, that information has been translated into five entries in the *Name Status (Validity)* table:
1. One for the current name with citation information: *Anadara camuloensis* (Osmont), Woodring, 1938, p. 29, pl. 6, figs. 10, 13-16; Winterer & Durham, 1962, table 4
1. One for the first synonym with citation information: *Arca camuloensis* Osmont, 1905
1. One for the second synonym with citation information: *Larkinia camuloensis*  (Osmont)
1. One for the third synonym with citation information: *Anadara (Larkinia) camuloensis* (Osmont), Durham & Addicott, 1965, table 1
1. One for all other synonyms that do not yet have citation information: *Arca (Larkinia) camuloensis*, *Arca (Arca) multicostata camuloensis*

{% include figure image_path="/assets/images/epicctaxonomy_history1.png" alt="screenshot of the Validity tab in EMu showing taxonomic name history" caption="Screenshot of taxonomic name history for *Anadara camuloensis* captured on the *Validity* tab of the Taxonomy module. The highlighted entry here illustrates how information for the current name (*Anadara camuloensis*) is captured." %}

{% include figure image_path="/assets/images/epicctaxonomy_history2.png" alt="screenshot of the Validity tab in EMu showing taxonomic name history" caption="Screenshot of taxonomic name history for *Anadara camuloensis* captured on the *Validity* tab of the Taxonomy module. The highlighted entry here illustrates how information for a synonym name that has citation details is captured." %}

{% include figure image_path="/assets/images/epicctaxonomy_history3.png" alt="screenshot of the Validity tab in EMu showing taxonomic name history" caption="Screenshot of taxonomic name history for *Anadara camuloensis* captured on the *Validity* tab of the Taxonomy module. The highlighted entry here illustrates how information for any additional synonym names that do **not** have citation details is captured. These names can eventually be parsed out of this entry and recorded separately on their own as the citation details are tracked down." %}

Please note that the order of the rows in the *Name Status (Validity)* table should be chronological by historic use, but that in the process of migrating the taxonomic dictionary that order was not preserved perfectly. Re-ordering the rows is as simple as clicking the lefthand side (where each row is numbered) and dragging it up or down.

## Descriptions tab

The following columns were migrated to the *Descriptions* tab in EMu, and will move to a new tab (*Ecology*) in the pending EMu update:
- *Age Range*
- *Geog. Range*
- *Type No.*
- *L*, *W*, and *H*
- *Recent Dist*
- *High Lat* and *Low Lat*
- *Min Depth* and *Max Depth*
- *Zone*
- *Substrate*
- *Abundance*
- *Min Temp* and *Max Temp*

{% include figure image_path="/assets/images/epicctaxonomy_descriptions.png" alt="Descriptions tab of the EMu taxonomy module" caption="Screenshot of the *Descriptions* tab of the Taxonomy module, showing various attributes for an EPICC name." %}

Other attributes were not migrated into EMu either because the field held a calculated value (e.g. *Mean Depth*) or because the field was related to a specific project that did not need to be carried forward into EMu (e.g. *Extinction*).
