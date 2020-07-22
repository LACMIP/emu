---
title: Digitizing
navcat: Workflows
tags: cataloging, georeferencing
last_modified_at: 2020-07-15
---

Multiple grants from the National Science Foundation support current digitization initiatives at LACMIP. "Digitization" itself is a broad term and includes the variety of workflows outlined here. For a more thorough review of digitization workflows, see [Nelson *et al.* 2012](https://doi.org/10.3897/zookeys.209.3135).

# Pre-digitization

## Pre-digitization workflow

Pre-digitization is completed by LACMIP staff. 

 *Step* | *Pre-digitization task...*
   --- | ---
   1 | <img src="{{ site.baseurl }}/assets/images/digitizing_worksheetexample2.png" alt="" width="500"/>{: .align-center} **Select specimens.** Using the stratigraphic collections inventory, select a tray from the collection to be digitized and immediately begin a [new digitization worksheet](https://github.com/LACMIP/emu/blob/master/docs/assets/images/digitizing_digitzationworksheet2020.pdf). Every tray to be digitized will receive a worksheet upon removal from the collection; these workheets must remain with the tray until the digitization process is complete.
   2 | **Verify localities.** Before identifying and rehousing any specimens, check that all associated locality information in EMu is complete and accurate. The fields that will most likely require attention are the _Geographic Details_ and _Collectors_. Filling out these fields will ensure labels will be complete upon printing. Refer to the instructions on [entering new geographic data](https://lacmip.github.io/emu/documentation/sites/#entering-new-geographic-data) and the [IP Locality (1) tab](https://lacmip.github.io/emu/documentation/sites/#ip-locality-1-tab) if _City/Town_ or _Nearest Place_ are blank. If the _Collectors_ _Names_ or _Start Date/End Date_ fields are blank, look for this information on the [Notes tab](https://lacmip.github.io/emu/documentation/sites/#notes-tab) in the Sites module, as well as on old locality cards in the tray. Fill in this information using the “Firstinitial Lastname” format. If the collector is truly unknown, fill in this field with “unknown” in EMu. Collecting dates may be left blank if they are unknown.
   3| <img src="{{ site.baseurl }}/assets/images/digitizing_localitycard.png" alt="" width="500"/>{: .align-center} **Generate new IP Locality Cards.** Once vetted, run the “IP Locality Cards” report in EMu’s Sites module for all localities in the tray. Print the card(s) on archival paper, plasticize and seal them, and then neatly tuck the card(s) under the specimen boxes in the tray.
   4 | **Sort, identify, and rehouse specimens.** Identifications should be made using the most current taxonomic dictionary available for that fauna. Refer to the [identification](https://lacmip.github.io/emu/documentation/digitizing/#identification-guidelines) and [rehousing](https://lacmip.github.io/emu/documentation/digitizing/#rehousing-guidelines) guidelines below.
   5 | **Return uncataloged tray to the collection.** Follow [these instructions](https://lacmip.github.io/emu/documentation/digitizing/#returning-uncataloged-trays).
   
## Identification guidelines

<img src="{{ site.baseurl }}/assets/images/digitizing_idtagexample.jpg" alt="" width="600"/>{: .align-center}
- Every distinct taxon that can be identified will receive its own specimen [ID tag](https://lacmip.github.io/emu/documentation/cataloging/#id-tag-anatomy). For older (non-Plio-Pleistocene) collections, specimens are commonly lithified together, meaning multiple tags may be necessary per box. Stack the tags in the order that you would like the specimens cataloged (i.e., first tag on top will be cataloged first).
- Take care to record old (“alt”) catalog numbers from UCLA, CIT, etc. (Ask if you’re unsure whether a number is an old catalog or locality number.)
<img src="{{ site.baseurl }}/assets/images/catalogue_alternativenumbersexample.jpg" alt="" width="600"/>{: .align-center}
- _Assume you will not be available if the cataloger has questions._ Therefore, clearly indicate what fields additional information should be entered into, e.g. *ID Comments*, if extensive remarks are made on the back of an ID tag.
- If the specimen’s _Original Nature_ is not “body fossil” and/or the _Anatomy_ is not “shell(s)”, write this information in the space above “New ID”.
<img src="{{ site.baseurl }}/assets/images/digitizing_flexspace.png" alt="" width="500"/>{: .align-center}
- In addition to ID tags, [blue “TX” tags](https://github.com/LACMIP/emu/blob/master/docs/assets/images/digitizing_txtagstemplate.pdf) should also be completed for all lots destined for the taxonomic collection. Further, if associated lots are to be sent to the taxonomic collection in the same box (e.g., a bivalve with an associated boring), include both catalog numbers on the tag.
<img src="{{ site.baseurl }}/assets/images/digitizing_txtags.png" alt="" width="500"/>{: .align-center}

## Rehousing guidelines
- Rehouse all lots destined for the **ST** collection in **short-sided boxes**. Occasionally, exceptions are made for large lots that might easily spill out of short-sided boxes.
- Rehouse all lots destined for the **TX** collection in **tall-sided boxes**.
- Smaller specimens and lots that comfortably fit in vials should be rehoused as such.
- Avoid needlessly splitting lots to keep specimens from expanding into neighboring trays (and _especially_ drawers) when possible. Consider designating a few additional specimens as "TX" if that will ultimately mitigate tray overflow into another drawer.

When all specimen sorting, identification, and rehousing is complete, arrange all boxes in this order:
{% include figure image_path="/assets/images/digitizing_trayarrangement.jpg" alt="Example of how to arrange a specimen lots in a tray. Right-click the image above to enlarge it in a separate tab or window." caption="Once you finish identifying the specimens in a tray, arrange the boxes by locality and taxon. " %}
- **Primarily by locality.** Do not intermix lots from different localities within the tray.
- **Secondarily by taxon.** Beginning with lots containing bivalves, arrange the boxes from left to right (and back to front) in this order: _Bivalvia > Gastropoda > Other Mollusca > Other taxa & trace fossils_
- If a box contains multiple lots (e.g., a bivalve and gastropod), arrange the box according to whichever specimen you deem to be most significant.
- Taxa from the same family should be placed together, e.g. keep all Veneridae lots from the same locality together.
- **All TX lots should be placed together**; this helps ensure that these lots will be correctly entered as “ST” or “TX” during cataloging, as do the blue TX tags.
- Lastly, if you decide some specimens should not be cataloged, they should remain separated by locality, but condensed, if possible. Place these boxes at the far right of the tray. For these lots, add an ID tag with the locality number followed by an “X” (e.g. “LACMIP 12345.X”) and write “do not catalog” in the space for New Name.

## Returning uncataloged trays
After all specimen lots in a tray have been sorted, identified, and rehoused, they must be returned to the collection until someone is available to catalog them.
- In EMu’s Locations module, search: _Level 3_ = cabinet # & _Level 4_ = drawer #
<img src="{{ site.baseurl }}/assets/images/digitizing_relocating1.png" alt="" width="700"/>{: .align-center}
- Open the record for the drawer and navigate to the Notes tab.
- Begin (or continue) a list of trays in the drawer that are ready for cataloging in this format: “YYYY MM DD - YourName”
- If you identified multiple trays from the same drawer on the same day, add a letter to the date on the worksheet and in EMu.
<img src="{{ site.baseurl }}/assets/images/digitizing_relocating2.png" alt="" width="700"/>{: .align-center}

Leave the digitization worksheet in the tray when you return it to the collection.
{: .notice--warning}

# Digitization

There are three major components of the LACMIP digitization workflow: cataloging, georeferencing, and imaging. Most of these activities are completed by volunteers or interns.

## Cataloging

Before you begin cataloging, add your name and the date to the _Count+Catalog_ field on the tray's digitization worksheet:
<img src="{{ site.baseurl }}/assets/images/cataloging_digitizationworksheet.png" alt="" width="500"/>{: .align-center}

See separate documentation for the complete [cataloging workflow]({{ site.baseurl }}/documentation/cataloging/).

### Counting

Check that *Count* is filled out on all ID tags. If it's blank, you'll need to complete this information before or during cataloging.
<img src="{{ site.baseurl }}/assets/images/digitizing_lotcount.jpg" alt="" width="400"/>{: .align-center}
A few tips for counting...
- Every separate and distinct piece of material counts as one specimen. For example, the _Lot Count_ for the sample below is "1", even though it has multiple shells stuck to it.
<img src="{{ site.baseurl }}/assets/images/digitizing_countingexample.png" alt="" width="500"/>{: .align-center}
- Very small and incomplete fragments should not be counted. Ask if you are unsure when a fragment is too small to count.
- Unsorted fossils and unsorted sediment always has a count of one.
- If a bivalve is articulated (i.e. the valves are attached to each other), both valves are counted as individual specimens **unless** the bivalve is an internal mold (i.e. the impression of a fossil with no shell left). This is not common in the older parts of the collection.
- The easiest method for counting large lots is to group specimens in piles of 10 and then tally the piles.

## Georeferencing

See separate documentation for [georeferencing]({{ site.baseurl }}/documentation/georeferencing/). Georeferencing can occur at any point in the digitization workflow, but preferably before labels are printed.

## Imaging

Specimen image capture and processing are essential components of digitization. Complete documentation for this step is forthcoming. The current protocol for imaging insect compression fossils can be accessed [here](https://github.com/LACMIP/emu/blob/master/docs/assets/images/LACMIP_Compression_Fossil_Imaging_Protocol.pdf).

# Post-digitization curation

Physical curation is an important component of the overall digitization process, not only because it increases digitization efficiency, but also because it provides the opportunity to improve things such as taxonomic identifications, physical storage conditions, etc.

## Painting
Most LACMIP specimens already have locality numbers glued or painted on them. For this reason, the need for painting is limited. This step is mostly completed by IP staff following cataloging. A few tips for painting...
- All **vials** should be painted with a stripe extending ~3/4" from the bottom and is ~1/8" wide. The "stripe checker" tool, as seen in the image here, can help guide you when you are new to this step.
<img src="{{ site.baseurl }}/assets/images/digitization_stripechecker.jpg" alt="" width="400"/>{: .align-center}
- If a specimen has **multiple ID tags** (indicating multiple lots), you will need to **paint multiple stripes** to provide space for each catalog number on vials and plastic boxes. Typically one stripe per catalog number is fine, but if you have a specimen with an excessive amount of lots, please ask LACMIP staff for advice. Additional stripes are always painted below one another on vials.
- **Do not paint loose specimens**. LACMIP staff will determine whether this is necessary.
- Steady each specimen or vial against the table to help paint smooth, clean stripes.
- Stand vials on their lids (upside-down) to dry.
- Paint should left to dry for 24 hours prior to numbering.

Do not let paint dry to your brush! This will ruin it. Keep a water cup and paper towel handy for quick cleaning. As soon as you have finished painting or need to take a break, wash your brush thoroughly. 
{: .notice--warning}

## Numbering

About 24 hours after painting, vials can be numbered. The **#1 rule** of numbering specimens is that **neatness counts**! Use either a 01 or 005 black Pigma Micron pen to number.

{% include figure image_path="/assets/images/digitization_numbering.png" alt="" caption="Letters and numbers should be written according to this example. Do not cross '7' or enclose the number '4'" %}

A few tips for numbering...
- Press lightly and use short pen strokes, somewhat as though you are "painting" the letters and numbers on.
- Steady the vial against a hard surface.
- Avoid touching the ink before it’s dried.
- If a lot has more than one catalog number, both need to be written on the vial. 

Wait at least 24 hours after painting to number vials; using Micron pens on semi-dry paint will ruin them.
{: .notice--warning}

## Labels

<img src="{{ site.baseurl }}/assets/images/digitization_labels.jpg" alt="" width="300"/>{: .align-right}

Once specimens have been cataloged, new labels are printed and must be cut/placed before the specimen tray can return to its permanent storage location. The image to the right depicts an example of a newly-labeled specimen. Labeling involves the following steps...
1. Use the paper cutter to cut labels neatly, leaving a thin border around the black outline. **Never cut more than once sheet of labels at a time**.
1. Separate ST/TX labels and arrange each pile in numerical order by locality number.
1. Find the tray of specimens to which the labels belong. Match each label to its specimen, then either neatly fold on the dotted line and place the label inside the specimen box (for lots housed loose or in small vials) **or** neatly cut on the dotted line and place the label inside the specimen vial (for EPICC lots housed in medium and large vials). Note that...
    - non-EPICC lots may not need to have their label cut and placed inside the vial; please check with LACMIP staff
    - Some boxes will require multiple labels (one per lot).
    - Left-justify labels, with additional labels visible to the right when they are present.
    - When placing the label inside a vial, always remove specimens first, and orient the ST/TX box on the label at the bottom of the vial (away from the cap).
    - Never force specimens back into a vial. They need to have some breathing space. If you are struggling to get all of the specimens back into the vial after putting the label in, ask for help.
    - In the case of TX specimens, whenever possible place all relevant tags and labels inside the vial with the specimens. Only do this if you can do so without damaging the specimens or paper.
    - Older labels should not be removed from their boxes. This includes the handwritten labels, as well as labels on printer paper (c. 2004-2013) and new ID tags.
    - Watch for labels with missing/incorrect information as they will need reprinting! It is especially important to spot check the lot count and taxonomic identification between the handwritten ID tag and the printed label.

## Relocating

{% include figure image_path="/assets/images/digitizing_rehousing.jpg" alt="Example of how to rehouse specimen lots in a tray." caption="When digitization is complete, your tray should look something like this." %}
