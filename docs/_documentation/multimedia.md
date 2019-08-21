---
title: Multimedia
navcat: Modules
tags: imaging
toc: false
last_modified_at: 2019-02-01
---
The Multimedia module records metadata about media uploaded to EMu, either in batch (e.g. specimen images) or on the fly (e.g. a screenshot of a taxon from a publication). These records can then be connected to other records, primarily Catalogue, Taxonomy, and Sites. Please see [Axiell's documentation](http://help.emu.axiell.com/latest/en/Topics/Common/Multimedia%20module.htm) for generic information about this module.

{% include figure image_path="/assets/images/multimedia_multimedia.png" alt="screenshot of multimedia module" caption="Multimedia module in EMu." %}

LACMIP does not use EMu as a DAMS, and therefore only a skeleton crew of fields (highlighted in the figure above) should be used within the Multimedia module. *MIME Type*, *MIME Format*, and *Identifier* are all automatically generated, and the only additional field we recommend using is *Title*, where you should put something descriptive. Although it may be tempting to fill out information in the other fields and tabs, keep in mind that if you do it is likely to be a waste of time since the Multimedia module is not being systematically managed as a repository for data (only media).

As of 2019, LACMIP's strategy has been to manage media metadata via the EXIF information embedded within the file itself. EMu imports the EXIF metadata into an *EXIF* tab and this information is searchable via the *Value* field.

{% include figure image_path="/assets/images/multimedia_exif.png" alt="screenshot of multimedia module exif tab" caption="EXIF tab in the Multimedia module." %}

Information about managing media and how it is published can be found under [Publishing Data](https://lacmip.github.io/emu/documentation/ipt/).
