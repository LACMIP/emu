---
title: Re-identifications
navcat: Workflows
tags: taxonomy
---
Whether because of evolving taxonomy or differing expert opinions, re-identifying specimens is a constant aspect of maintaining biological collections. LACMIP maintains a record of past and present identifications in the [Catalogue module]({{ site.baseurl }}/documentation/catalogue/) of EMu.

## Individual specimen re-identification

To update the taxonomic identification of an individual specimen, navigate to the *Identification (1)* tab of the specimen's catalogue record and enter the information described here:
- *Taxon*: attach the taxonomy record for the new identification
- *Modifier*: if the specimen has a taxonomic modifier, e.g. "cf.", enter it here
- *Modifier Rank*: tell EMu which part of the scientific name the modifier applies to, e.g. "species" for an identification of "Glycymerita cf. veatchii"
- *Identified By*: enter the full name of the identifier, e.g. "Austin Hendy"
- *Identified Date*: pick the date of the identification
- *Comments*: if there are any comments, enter them here
- *ID Reference*: attach this identification to a bibliography record, if applicable (rare)
- *Filed As?*: enter the same value you enter for *Currently Accepted?*
- *Currently Accepted?*: enter "Yes" if you are updating the identification to a current name; enter "No" if you are adding an old identification to the catalogue record

{% include figure image_path="/assets/images/reidentify_screenshot.png" alt="identification tab" caption="Screenshot of the *Identification (1)* tab in the Catalogue module of EMu. If you need to  look up the current name, you can easily see it by going to the taxonomy record of the old identification, as indicated by the arrows above. Also noticed that the *Modified Taxon* field is grayed out because it is constructed automatically by EMu." %}

Make sure to save your changes, and to [print new labels]({{ site.baseurl }}/documentation/labels/) if you are also updating the physical specimen.

## Bulk re-identification

<img src="{{ site.baseurl }}/assets/images/reidentify_search.png" alt="" width="300"/>{: .align-right}
When taxonomy itself changes, you may want to use EMu's *Re-identify* tool to update the catalogue records in bulk. Begin by searching for the scientific name that you want to update in the *Modified Taxon* field of the Catalogue module search, and selecting the resulting records.

{% include figure image_path="/assets/images/reidentify_tool.png" alt="re-identification tool" caption="Screenshot of the EMu Catalogue module illustrating how to find the re-identification tool under *Tools > Re-identify*. " %}

The *Re-identify* tool allows you to choose between affecting the *Current Record* or *Selected Records*. For taxonomic name updates, you'll likely want to use *Selected Records*, with all of the records in your search results included.

<img src="{{ site.baseurl }}/assets/images/reidentify_dialog.png" alt="" width="400"/>{: .align-right}
In the new window that EMu brings up, enter all of the same information as you are used to entering at the specimen level. **For bulk re-identifications, you should include a comment if you did not look at each specimen.**(Suggested comment: "Taxonomy updated, but specimen not examined.")Remember to change both *Currently Accepted?* and *Filed as?* to "Yes" if you are updating the identification to a current name or "No" if you are adding an old identification to the catalogue record. The only specimens where a single name should have different values for *Currently Accepted?* and *Filed as?* are types.

<img src="{{ site.baseurl }}/assets/images/reidentify_non-types.jpg" alt="" width="400"/>{: .align-center}
<img src="{{ site.baseurl }}/assets/images/reidentify_types1.jpg" alt="" width="400"/>{: .align-center}
<br>
<br>

## Checking data quality

Ideally we strive to only identify specimens with valid names, and to re-identify affected specimens any time we updated our taxonomic dictionary. Nonetheless, it is advisable to **periodically check for specimens that lack a valid identification**. To do so...

1. Pull up all records in the Catalogue module by leaving every search field empty.
1. Go to *File > Additional Search > Subtract (NOT)...*
1. In the additional search, go to the *Identification (1)* tab and click the green plus sign next to the *Taxon* field.
1. Search the Taxonomy module for all records where *Currently Accepted?* = "Yes."
1. Attach **all** of the resulting taxonomy records and complete your additional search.

The resulting catalogue records should be all those that are **not** attached to an accepted taxonomic name. This is a computationally expensive search and will likely take EMu 10+ minutes to do. This search is not perfect, as it leaves out records where the accepted identification is not a valid name but previous identifications have been, e.g.:

```
Current ID: Yaadia hemphilli (an unaccepted name)
Old ID: Yaadia sp. (where Yaadia is an accepted genus)
```

You can use the re-identify tool to update specimen records returned by this search. 
