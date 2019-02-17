---
title: Catalogue
navcat: Modules
tags: cataloging quick-start
---
The Catalogue module is the primary place for information about each specimen lot, and a node linking together data from many of the other modules. Please see [Axiell's documentation](http://help.emu.axiell.com/latest/en/Topics/EMu/Catalogue%20module.htm) for generic information about this module.

See also [Cataloging Specimens]({{ site.baseurl }}/documentation/cataloging/)

## Invert. Paleo. tab

{% include figure image_path="/assets/images/catalogue_invertpaleo.png" alt="screenshot of the invert paleo tab in the catalogue module" caption="Screenshot of the *Invert. Paleo.* tab of the Catalogue module." %}

Fields on this tab are...

Locality
:

Lot Count
:

Disp.
:
    - "being processed"
    - "discarded"
    - "in collection"
    - "missing"
    - "on loan"
    - "unknown"

Lot No.
: turns into *Cat. No.*

P/CP
:

Accn. Lot
:

LACMIP Type No.
:

Field No.
:

Accn. No.
:

Inst. Code & Inst. Number
: "UCLA" or "Cerritos College" or "collector number" (e.g. "PIERCE NODULE 142")

Identification
: Displays *Modified Taxon*, *Identified By*, and *ID Date* from the other tab

Type Status
: controlled vocabulary

Collectors
: only use one row!

Collection
:
    - "ED"
    - "Other"
    - "ST"
    - "TX"
    - "Type"

Project
:
    - "CSC"
    - "EPICC"
    - "FIC"

Lot Remarks
: Some parts of the collection have more data than others (insects)

Publication
:

Pages
:

Fig.
:

Type
:

Original Nature
:
    - "body fossil"
    - "cast"
    - "compression fossil"
    - "encrustation"
    - "mold"
    - "slab"
    - "slide"
    - "synthetic"

Anatomy
: most mollusks will be "body"

## Identification (1) tab

{% include figure image_path="/assets/images/catalogue_identification.png" alt="screenshot of the identification tab in the catalogue module" caption="Screenshot of the *Identifications (1)* tab of the Catalogue module." %}

Fields on this tab are...

Taxon
: Link to the attached [Taxonomy]({{ site.baseurl }}/documentation/cataloging/) record.

Modifier
: Any part of the identification other than the taxonomic name, e.g. "cf." or "sp." or "indet." This is a controlled vocabulary; you can see the value options by clicking on the icon to the right of the field. Along with *Modifier Rank* and *Taxon*, this field gets arranged into *Modified Taxon*.

Modifier Rank
: If there is a value for *Modifier*, then EMu also needs this field to tell it where to place the modifier. For the modifiers "sp." and "indet." this should be the taxonomic rank of the lowest level included in *Taxon*. For identification qualification modifiers such as "cf." this should be the taxonomic rank before which the modifier gets place. For example...
    - for an identification of "Calva sp.": *Taxon* = "Calva" / *Modifier* = "sp." / *Modifier Rank* = "genus"
    - for an identification of "Veneridae indet.": *Taxon* = "Veneridae" / *Modifier* = "indet." / *Modifier Rank* = "family"
    - for an identification of "Calva cf. varia": *Taxon* = "Calva varia" / *Modifier* = "cf." / *Modifier Rank* = "genus"

Identified By
: Full name(s) of the person or people who made this identification, e.g. "LouElla Saul." For legacy data we frequently do not track this data.

Date Identified
: Date on which the identification was made. This can be as granular as a day (e.g. "3/20/2018") or as coarse as a year (e.g. "2018"). For legacy data we frequently do not track this data.

Comments
: Any comments about the identification.

ID Reference
: A bibliographic record related to the identification can be attached via this field, if desired.

Filed As
: This field should be "Yes" wherever *Currently Accepted* is also "Yes" and "No" wherever *Currently Accepted* is also "No," except for on the records of type specimens whose taxonomy is outdated (see [Re-identifications]({{ site.baseurl }}/documentation/reidentify/) for more on this).

Currently Accepted
: This field should be "Yes" for any identification attaching a current taxonomic name, and "No" for invalid taxonomy as well as legacy identifications. Only one identification can have a value of "Yes" for *Currently Accepted*, so even if a legacy identification is taxonomically valid, you need to enter "No" for this field.

## Location tab

LACMIP does not currently use the *Location* tab. It is designed to track physical specimen movement.

## Registrar tab

The *Registrar* tab contains information about the provenance and disposition of the physical specimen(s) and is maintained by the Museum's Registrar. Please do not edit fields on this tab.

## Multimedia tab

{% include figure image_path="/assets/images/catalogue_multimedia.png" alt="screenshot of the multimedia tab in the catalogue module" caption="Screenshot of the *Multimedia* tab of the Catalogue module." %}

If a specimen has been imaged, the image should be attached to the catalogue record. [Multimedia]({{ site.baseurl }}/documentation/multimedia/) attachments are visible on the *Multimedia* tab. In the screenshot above, you can see that the metadata from the multimedia record appears in the sidebar of this tab. Double-clicking on an image will open it in a larger viewer. Clicking on the green plus sign allows you to attach additional multimedia records.

## Admin

{% include figure image_path="/assets/images/catalogue_admin.png" alt="screenshot of the admin tab in the catalogue module" caption="Screenshot of the *Admin* tab of the Catalogue module." %}

The *Admin* tab contains information about the record's provenance and edit history. This can be a useful way to check when and by whom a record was created or most recently modified. This tab is also where the record's GUID, or Global Unique Identifier, is stored. For catalogue records this is a critical identifier that gets published with the specimen occurrence data and ensures users can trace the data back to its source (i.e. the catalogue record at LACMIP).

## Security

{% include figure image_path="/assets/images/catalogue_security.png" alt="screenshot of the security tab in the catalogue module" caption="Screenshot of the *Security* tab of the Catalogue module." %}

The only field you need to be concerned with on the *Security* tab is *Publish on Internet*, which should be check "Yes" for the majority of catalogue records but "No" for any records that should not be shared via biodiversity aggregators (e.g. iDigBio, GBIF). A record should be marked "No" either because the specimen or its data are questionable, or as part of a research moratorium pending publication. Specific examples include but not limited to:
- records where the specimen disposition is "missing"
- records where the specimen disposition is "discarded"
- records of type specimens of an unpublished new species
- records that may have been incorrectly catalogued

By default, EMu checks "Yes" for the *Publish on Internet* field. If you feel that a record should not be made public, please go to this tab and check "No."
