---
title: Catalogue
navcat: Modules
tags: cataloging quick-start
last_modified_at: 2019-03-01
---
The Catalogue module is the primary place for information about each specimen lot, and a node linking together data from many of the other modules. Please see [Axiell's documentation](http://help.emu.axiell.com/latest/en/Topics/EMu/Catalogue%20module.htm) for generic information about this module. Continue reading here to understand how LACMIP uses the fields available in the Catalogue module.

For detailed instructions on entering new records in this module, please [Cataloging Specimens]({{ site.baseurl }}/documentation/cataloging/) in addition to this page.

## Invert. Paleo. tab

{% include figure image_path="/assets/images/catalogue_invertpaleo.png" alt="screenshot of the invert paleo tab in the catalogue module" caption="Screenshot of the *Invert. Paleo.* tab of the Catalogue module." %}

This tab, along with *Identifications (1)*, is where the bulk of our specimen data lives. Fields on this tab are...

Locality
: Attach a [site]({{ site.baseurl }}/documentation/sites/) record to the catalogue record here. You can either type in the LACMIP locality number, e.g. "500000," or click the green plus sign to find a locality via the Sites module search.

Lot Count
: The number of individuals within this cataloged lot. Typically, this is the number of physical pieces, e.g. on a single chunk of Cretaceous material there may be thousands of individual fossilized animals but *Lot Count* would be "1." For more recent material, *Lot Count* may actually be the number of individual animals. It is important to ask for clarification on what this number means if you are unfamiliar with LACMIP norms.

Disp.
: A controlled vocabulary to note the physical state of a specimen lot. Vocabulary includes:
    - "being processed" for specimens actively being incorporated into the collection, e.g. a new donation
    - "discarded" for specimens permanently removed from the collection
    - "in collection" for specimens physically locatable
    - "missing" for specimens whose whereabouts are unknown
    - "on loan" for specimens out on loan
    - "unknown" for specimens that haven't been physically located, but are also not definitely missing; typically this term is assigned to legacy specimen data records where we have not attempted to locate the physical specimen yet

Lot No.
: Combined with the locality number, this turns into *Cat. No.*, a unique, human-readable identifier for a specimen lot. EMu will auto-generate the next available lot number for you.

P/CP
: Part/Counterpart. Checking this box indicates that the specimen lot contains two pieces which fit together to represent a single animal.

Accn. Lot
: Attach an accession record here. Most LACMIP specimens do not have accession information digitally available yet. Please contact the Museum registrar if you need to attach accession information that has not already been digitized. LACMIP staff do not have permission to add/modify records in the [Accession Lots module]({{ site.baseurl }}/documentation/accessions/).

LACMIP Type No.
: Specimens in the type collection have a type number; it should be recorded here.

Field No.
: A number assigned to a specimen lot **at the time of collection**, typically by the collector. This is not common in the majority of the LACMIP collections (fossil insects being an exception).

Accn. No.
: Do not use this field.

Inst. Code & Inst. Number
: Paired values of specimen numbers assigned **during curation** by another institution. For example, many UCLA specimens have numbers; "UCLA 1778" would be entered into EMu as *Inst. Code* = "UCLA" and *Inst. Number* = "1778," or "PIERCE NODULE 142" would be entered into EMu as *Inst. Code* = "collector number" and *Inst. Number* = "PIERCE NODULE 142." Take care not to record **locality** numbers from other institutions here (record them in the [Sites module]({{ site.baseurl }}/documentation/sites/)).

Identification
: Displays *Modified Taxon*, *Identified By*, and *ID Date* from the *Identification (1)* tab (see below for details).

Type Status
: A controlled vocabulary to classify the kind of type specimen. Vocabulary includes:
    - "figured"
    - "holotype"
    - "hypotype"
    - "lectotype"
    - "neotype"
    - "paralectotype"
    - "paraleptotype"
    - "paratype"
    - "syntype"

Collectors
: The fields in this section–*Collector Name*, *Start Date*, and *End Date*–will be moved to the [Sites module]({{ site.baseurl }}/documentation/sites/) with the next EMu update. Until then, we do need information here for printing labels. Enter multiple collectors into the same *Collector Name* row, e.g. "LouElla Saul, Mary Ann Swanson." Enter different values for *Start Date* and *End Date* if you have a date range, e.g. "2/17/2019" and "2/20/2019", or the same value if there is no explicit range, e.g. "2/17/2019" and "2/17/2019," or "2019" and "2019." Do not use the *Uncertain* field, and do not use more than one row of this nested table.

Collection
: A controlled vocabulary to indicate which physical part of the collection this specimen lot should be housed in. Vocabulary includes:
    - "ED" for specimens in the Education Collection
    - "Other" for specimens of unexplained or extraordinary physical circumstances
    - "ST" for specimens in the Stratigraphic Collection
    - "TX" for specimens in the Taxonomic Collection
    - "Type" for specimens in the Type Collection (housed at the main Museum building)

Project
: A controlled vocabulary to group catalogue records by project. This is useful for tracking project headway, but not every specimen will need a value in this field. You can add values to this controlled vocabulary via the [Lookup Lists module]({{ site.baseurl }}/documentation/lookuplist/). Current vocabulary includes:
    - "CSC" for Cretaceous Seas of California (CSBR grant, 2016-2019)
    - "EPICC" for Eastern Pacific Invertebrate Communities of the Cenozoic (TCN grant, 2015-2020)
    - "FIC" for Fossil Insect Collaborative (PEN grant, 2017-2020)

Lot Remarks
: Space for comments that do not fit elsewhere. Some parts of the collection more commonly have information for this field than others, e.g. fossil insects tend to have lifestage and other extra notes to record here.

Successive lot remarks (i.e., remarks made on different days by different people) should be formatted as such: Firstname1 Lastname1, Year1: Remark1. Firstname2 Lastname2, Year2: Remark. Etc. For example: Mary Stecheson, 2013: Specimen broken in transit. Keana Tang, 2019: Specimen is countertype of LACMIP Type 2889.

IP Publications
: The fields in this section allow you to attach a [bibliography record]({{ site.baseurl }}/documentation/bibliography/) to the catalogue record. This is usually only appropriate for specimens that belong to the Type Collection. *Pages*, *Fig.*, and *Type* are all used to provide more details about the citation.

Original Nature
: A controlled vocabulary recording the kind of fossil present. It is possible to record more than one value (one per row), e.g. if you have a specimen lot that includes the body fossil as well as a cast of it. Vocabulary includes:
    - "body fossil"
    - "cast"
    - "compression fossil"
    - "encrustation"
    - "mold"
    - "slab"
    - "slide"
    - "synthetic"

Anatomy
: A controlled vocabulary describing the part of the individual present. Typically mollusks will just be "body." There are many options, which you can view by clicking on the icon to the right of the field. It is possible to record more than one value (one per row). You can add values to this controlled vocabulary via the [Lookup Lists module]({{ site.baseurl }}/documentation/lookuplist/).

## Identification (1) tab

{% include figure image_path="/assets/images/catalogue_identification.png" alt="screenshot of the identification tab in the catalogue module" caption="Screenshot of the *Identifications (1)* tab of the Catalogue module. Highlighting a row in the *Identification List* brings up more detailed information in the fields above." %}

This tab allows us to track identification history of a specimen lot. As illustrated in the figure above, it is a nested table where each row represents a unique identification event. If you are looking for information about adding identifications to multiple catalogue records at the same time, please read the [re-identifications]({{ site.baseurl }}/documentation/reidentify/) documentation. Fields on this tab are...

Taxon
: Attach a record from the [Taxonomy module]({{ site.baseurl }}/documentation/cataloging/). If you know the full name you wish to attach, type it into this field along with its rank (e.g. "calva varians species" or "bivalvia class") and EMu will find the record directly. If the name you enter has multiple taxonomy record options, EMu will bring those up for you to select from. You can also use the full features of the Taxonomy module search by clicking on the green plus sign.

Modifier
: Any part of the identification other than the taxonomic name, e.g. "cf." or "sp." or "indet." This is a controlled vocabulary; you can see the value options by clicking on the icon to the right of the field. Along with *Modifier Rank* and *Taxon*, this field gets arranged into *Modified Taxon*.

Modifier Rank
: If there is a value for *Modifier*, then EMu also needs this field to tell it where to place the modifier. For the modifiers "sp." and "indet." this should be the taxonomic rank of the lowest level included in *Taxon*. For identification qualification modifiers such as "cf." this should be the taxonomic rank before which the modifier gets placed. For example...
    - for an identification of "Calva sp.": *Taxon* = "Calva" / *Modifier* = "sp." / *Modifier Rank* = "genus"
    - for an identification of "Veneridae indet.": *Taxon* = "Veneridae" / *Modifier* = "indet." / *Modifier Rank* = "family"
    - for an identification of "Calva cf. varia": *Taxon* = "Calva varia" / *Modifier* = "cf." / *Modifier Rank* = "species"

Identified By
: Full name(s) of the person or people who made this identification, e.g. "LouElla Saul." For legacy data we frequently do not track this data.

Date Identified
: Date on which the identification was made. This can be as granular as a day (e.g. "3/20/2018") or as coarse as a year (e.g. "2018"). For legacy data we frequently do not track this data.

Comments
: Any comments about the identification.

ID Reference
: A [bibliography record]({{ site.baseurl }}/documentation/bibliography/) related to the identification can be attached via this field, if desired.

Filed As
: This field should be "Yes" wherever *Currently Accepted* is also "Yes" and "No" wherever *Currently Accepted* is also "No," **except** for the records of **type specimens with outdated taxonomy** (see [re-identifications]({{ site.baseurl }}/documentation/reidentify/) for more on this).

*Filed As* describes how the specimen is physically organized (filed) in the collection. This is why types, which may have had their taxonomy updated since their inital publication, are not always filed with a currently accepted name.

Currently Accepted
: This field should be "Yes" for any identification attaching a current taxonomic name, and "No" for invalid taxonomy as well as legacy identifications. Only one identification can have a value of "Yes" for *Currently Accepted*, so even if a legacy identification is taxonomically valid, you need to enter "No" for this field.

## Location tab

LACMIP does not use the *Location* tab yet. It is designed to track physical specimen movement.

## Registrar tab

The *Registrar* tab contains information about the provenance and disposition of the physical specimen(s) and is maintained by the Museum registrar. Please do not edit fields on this tab.

## Multimedia tab

{% include figure image_path="/assets/images/catalogue_multimedia.png" alt="screenshot of the multimedia tab in the catalogue module" caption="Screenshot of the *Multimedia* tab of the Catalogue module." %}

If a specimen has been imaged, the image should be attached to the catalogue record and visible as an attachment on the *Multimedia* tab. In the screenshot above, you can see that the metadata from the [multimedia record]({{ site.baseurl }}/documentation/multimedia/) appears in the sidebar of this tab. Double-clicking on an image will open it in a larger viewer. Clicking on the green plus sign allows you to attach additional multimedia records.

## Admin tab

{% include figure image_path="/assets/images/catalogue_admin.png" alt="screenshot of the admin tab in the catalogue module" caption="Screenshot of the *Admin* tab of the Catalogue module, highlighting provenance and GUID data." %}

The *Admin* tab contains information about the record's digital provenance and edit history. This can be a useful way to check when and by whom a record was created or most recently modified. This tab is also where the record's GUID, or Global Unique Identifier, is stored. For catalogue records this is a critical identifier that gets published with the specimen occurrence data and ensures users can trace the data back to its source (i.e. the catalogue record at LACMIP).

## Security tab

{% include figure image_path="/assets/images/catalogue_security.png" alt="screenshot of the security tab in the catalogue module" caption="Screenshot of the *Security* tab of the Catalogue module." %}

The only field you need to be concerned with on the *Security* tab is *Publish on Internet*, which should be check "Yes" for the majority of catalogue records but "No" for any records that should not be shared via biodiversity aggregators (e.g. iDigBio or GBIF; for more see [Publishing Data]({{ site.baseurl }}/documentation/ipt/)). A record should be marked "No" either because the specimen or its data are questionable, or as part of a research moratorium pending publication. Specific examples include but are not limited to:
- records where the specimen disposition is "missing"
- records where the specimen disposition is "discarded"
- records of type specimens of an unpublished new species
- records representing unsorted fossils
- records that may have been incorrectly catalogued

By default, EMu checks "Yes" for the *Publish on Internet* field. If you feel that a record should not be made public, please go to this tab and check "No."

## Auxiliary tab

Only one field (*Aux. Rem 1*) on this tab is used, storing the *SpecIRN* value for catalogue records migrated from Access.
