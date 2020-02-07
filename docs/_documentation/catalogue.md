---
title: Catalogue
navcat: Modules
tags: cataloging quick-start
last_modified_at: 2020-02-07
---
The Catalogue module is the primary place for information about each specimen lot, and a node linking together data from many of the other modules. Please see [Axiell's documentation](http://help.emu.axiell.com/latest/en/Topics/EMu/Catalogue%20module.htm) for generic information about this module. Continue reading here to understand how LACMIP uses the fields available in the Catalogue module.

For detailed instructions on entering new records in this module, please [Cataloging Specimens]({{ site.baseurl }}/documentation/cataloging/) in addition to this page.

## Invert. Paleo. tab

{% include figure image_path="/assets/images/catalogue_invertpaleo.png" alt="screenshot of the invert paleo tab in the catalogue module" caption="Screenshot of the *Invert. Paleo.* tab of the Catalogue module. Users in the *Invertebrate Paleontology* and *IP Cataloging* permission groups have certain fields highlighted to assist with data entry. The Museum's database manager can adjust this or other field highlighting as desired." %}

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
    - "on loan" for specimens out on loan (refer to [transactions]({{ site.baseurl }}/documentation/transactions/) for more on loans)
    - "unknown" for specimens that haven't been physically located, but are also not definitely missing; typically this term is assigned to legacy specimen data records where we have not attempted to locate the physical specimen yet

Lot No.
: Combined with the locality number, this turns into *Cat. No.*, a unique, human-readable identifier for a specimen lot. EMu will auto-generate the next available lot number for you. If EMu does *not* automatically generate the *Lot No.*, do not proceed with cataloging and immediately alert the collections staff!

P/CP
: Part/Counterpart. Checking this box indicates that the specimen lot contains two or more pieces that fit together to represent a single animal. This is typically reserved for complete part-counterpart pairs of compression fossils and concretions.

Accn. Lot
: Attach an accession record here. Most LACMIP specimens do not have accession information digitally available yet. Please contact the Museum registrar if you need to attach accession information that has not already been digitized. LACMIP staff do not have permission to add/modify records in the [Accession Lots module]({{ site.baseurl }}/documentation/accessions/).

LACMIP Type No.
: Specimens in the type collection have a type number; record this information here. LACMIP type numbers are labelled on specimens in bright red, yellow, or blue paint. If you are unsure whether a number is a type number, consult the Collections Manager.
{% include figure image_path="/assets/images/catalogue_LACMIPtypeno.png" alt="example LACMIP Type No." caption="LACMIP type numbers are indicated by bright red, yellow, or blue paint. Red = holotypes, syntypes, lectotypes; Yellow = paratypes, paralectotypes; Blue = hypotypes (figured or unfigured specimens)." %}

Field No.
: A number assigned to a specimen lot **at the time of collection**, typically by the collector. This is not common in the majority of the LACMIP collections (fossil insects being an exception).

Accn. No.
: Do not use this field.

Inst. Code & Inst. Number
: Paired values of specimen numbers assigned **during curation** by another institution or the collector. For example, many UCLA specimens have old catalog numbers pasted onto them (white paper rectangles), such as "UCLA 4539". In this case, enter this number into EMu as *Inst. Code* = "UCLA" and *Inst. Number* = "4539." For specimen numbers assigned by the collector, such as "McK 227" assigned by W. D. Pierce, *Inst. Code* = "collector number" and *Inst. Number* = "PIERCE McK 227". Take care **not** to record **locality** numbers from other institutions in this field (record them in *Alternate Loc ID* in the [Sites module]({{ site.baseurl }}/documentation/sites/)).
{% include figure image_path="/assets/images/catalogue_alternativenumbers.png" alt="screenshot of the *Alternative Numbers* field in the catalogue module" caption="Screenshot of the *Alternative Numbers* field in the Catalogue module." %}
{% include figure image_path="/assets/images/catalogue_alternativenumbersexample.jpg" alt="Example of an old catalog number to be entered in *Alternative Numbers*" caption="Example of an old catalog number to be entered in *Alternative Numbers*" %}

Identification
: Displays *Modified Taxon*, *Identified By*, and *ID Date* from the *Identification (1)* tab (see below for details).

Type Status
: A controlled vocabulary to classify the kind of type specimen. Please enter the type status of highest priority that applies to the specimen. (For example, choose "holotype" or "syntype" over "hypotype"). The controlled vocabulary includes:
    - "allotype"
    - "holotype"
    - "hypotype" (to replace "figured")
    - "lectotype"
    - "neotype"
    - "paratype
    - "paralectotype"
    - "paraleptotype"
    - "paratype"
    - "syntype"
    - "unpublished type" (see _IP Publications_ below)

Collection
: A controlled vocabulary to indicate which physical part of the collection this specimen lot should be housed in. Vocabulary includes:
    - "ED" for specimens in the Education Collection
    - "Other" for specimens of unexplained or extraordinary physical circumstances
    - "ST" for specimens in the Stratigraphic Collection
    - "TX" for specimens in the Taxonomic Collection
    - "TYPE" for specimens in the Type Collection (housed at the main Museum building)
    - "GEO" for records representing derivative samples collected from ST/TX/TYPE specimens (for example, powdered aragonite to be used in destructive analysis). Records created for "GEO" samples should be related to the records for specimens from which they were derived à la (the Relationships tab)[https://lacmip.github.io/emu/documentation/relationships/].
    

Project
: A controlled vocabulary to group catalogue records by project. This is useful for tracking project headway, but not every specimen will need a value in this field. You can add values to this controlled vocabulary via the [Lookup Lists module]({{ site.baseurl }}/documentation/lookuplist/). Current vocabulary includes:
    - "EPICC" for Eastern Pacific Invertebrate Communities of the Cenozoic (TCN grant, 2015-2020)
    - "CSC" for Cretaceous Seas of California (CSBR grant, 2016-2019)
    - "Paleozoic" for ongoing (unfunded) digitization (2016-present)
    - "FIC" for Fossil Insect Collaborative (PEN grant, 2017-2020)
    - "WIS" for Cretaceous Western Interior & Pacific Northwest (PEN grant, 2019-2021)

Lot Remarks
: **#1 Rule for *Lot Remarks*: Avoid entering data into this field unless you are 100% certain the information is new AND cannot be recorded anywhere else in EMu.** In other words, this field provides space for recording data or comments for which an appropriate field does not yet exist. To facilitate future migration of data in *Lot Remarks* to more appropriate fields that do not yet exist, information added to this field should should be entered exactly as shown below (order matters, as well as capitalization and punctuation/separators). Please consult the Collections Manager if you are unsure whether you have information that should be added to *Lot Remarks*.
    - LIFESTAGE should be recorded verbatim.
    - SEX should be recorded verbatim, but do not abbreviate, e.g. "female" (not "f").
    - VERBATIM REMARKS ON SPM refers to any data written on the specimen or its label that should be recorded, but does not fit in any other field. Note that comments relating to the identification of a specimen do not go in *Lot Remarks*, but in the appropriate *Comments* field on the *Identification (1)* tab.
{% include figure image_path="/assets/images/catalogue_lotremarks.png" alt="screenshot of the *Lot Remarks* field in the catalogue module" caption="Screenshot of the *Lot Remarks* field in the Catalogue module." %}
    
IP Publications
: The fields in this section allow you to attach a [bibliography record]({{ site.baseurl }}/documentation/bibliography/) to the catalogue record. This is usually only appropriate for specimens in the Type Collection. Publications in this table should be listed chronologically with the oldest (first) publication appearing at the top of the list; you can click and drag to reorder these entries if needed. Data entered into each field should be formatted as follows:
    - *Pages*: Enter the page number(s) where the specimen is described. Do not enter "p.", "pg.", etc. before the number(s).
    - *Fig*: Enter the plate and figure number(s) separated by a colon. For example: "pl. 1: fig. 1-3". If a specimen is figured on multiple plates, separate these entries with a semicolon. For example, "pl. 1: fig. 1-5; pl. 4: fig. 3b, 3c". If the figure is unnumbered, enter "fig. unnumbered". If the specimen is unfigured, enter "unfigured".
    - *Type*: Indicate what kind of type the specimen is according to the publication. "Unpublished type" is reserved for specimens referenced in theses, dissertations, and historic manuscripts that will never be published.

{% include figure image_path="/assets/images/catalogue_IPpublications.png" alt="screenshot of the IP Publications field in the catalogue module" caption="Publications that reference LACMIP specimens by catalog or type number must be chronologically documented in the *IP Publications* table." %}

Original Nature
: A controlled vocabulary recording the kind of fossil present. It is possible to record more than one value (one per row) per catalog record, e.g. if you have a specimen lot that includes the body fossil as well as a cast or latex peel associated with it. Vocabulary includes:
    - "body fossil"
    - "boring"
    - "bulk" (to indicate the lot includes unsorted specimens or similar material)
    - "cast" (applies to natural casts, not man-made)
    - "compression fossil"
    - "concretion"
    - "encrustation"
    - "ichnofabric"
    - "micromount"
    - "mold" (applies to natural molds, not man-made)
    - "slab"
    - "slide"
    - "synthetic" (applies to facsimiles, e.g., plaster casts and rubber peels).
    - "trackway"

Anatomy
: A controlled vocabulary describing the part of the individual present. Typically, mollusks will just be "shell(s)." There are many options, which you can view by clicking on the icon to the right of the field. It is possible to record more than one value (one per row). You can add values to this controlled vocabulary via the [Lookup Lists module]({{ site.baseurl }}/documentation/lookuplist/). Leave this field blank for trace fossils.

## Identification (1) tab

{% include figure image_path="/assets/images/catalogue_identification.png" alt="screenshot of the identification tab in the catalogue module" caption="Screenshot of the *Identifications (1)* tab of the Catalogue module. Highlighting a row in the *Identification List* brings up more detailed information in the fields above." %}

This tab allows us to track identification history of a specimen lot. As illustrated in the figure above, it is a nested table where each row represents a unique identification event. If you are looking for information about adding identifications to multiple catalogue records at the same time, please read the [re-identifying]({{ site.baseurl }}/documentation/reidentify/) documentation. Fields on this tab are...

Taxon
: Attach a record from the [Taxonomy module]({{ site.baseurl }}/documentation/cataloging/). If you know the full name you wish to attach, type it into this field along with its rank (e.g. "calva varians species" or "bivalvia class") and EMu will find the record directly. If the name you enter has multiple taxonomy record options, EMu will bring those up for you to select from. You can also use the full features of the Taxonomy module search by clicking on the green plus sign.

Modifier
: Any part of the identification other than the taxonomic name, e.g. "cf." or "sp." or "indet." This is a controlled vocabulary; you can see the value options by clicking on the icon to the right of the field. Along with *Modifier Rank* and *Taxon*, this field gets arranged into *Modified Taxon*. EMu should automatically complete this field for you.

Modifier Rank
: If there is a value for *Modifier*, then EMu also needs this field to tell it where to place the modifier. For the modifiers "sp." and "indet." this should be the taxonomic rank of the lowest level included in *Taxon*. For identification qualification modifiers such as "cf." this should be the taxonomic rank before which the modifier gets placed. EMu should automatically complete this field for you. The logic behind this field is as follows:
    - for an identification of "Calva sp.": *Taxon* = "Calva" / *Modifier* = "sp." / *Modifier Rank* = "genus"
    - for an identification of "Veneridae indet.": *Taxon* = "Veneridae" / *Modifier* = "indet." / *Modifier Rank* = "family"
    - for an identification of "Calva cf. varia": *Taxon* = "Calva varia" / *Modifier* = "cf." / *Modifier Rank* = "species"
    - for an identification of and ichnotaxon (*Kingdom* = "Ichnotaxa"): *Taxon* = "Oichnus" / *Modifier* = "isp." / *Modifier Rank* = "genus"

Identified By
: Full name(s) of the person(s) who made this identification, e.g. "LouElla Saul." For multiple identifiers, please use initials rather than full names, e.g. "L. R. Saul, J. Alderson". **Note:** If you are *updating or verifying the taxonomy of a specimen, but not physically/critically examining it*, also enter "Taxonomy verified." or "Taxonomy updated." in *Comments*. Likewise, *ID Reference* should also be completed for taxonomic updates and verifications.

Date Identified
: Date on which the identification was made. This can be as granular as a day (e.g. "3/20/2018") or as coarse as a year (e.g. "2018"). For historic identifications (i.e., pre-2015), you may leave this field blank if no identification date has been clearly indicated on the specimen label.

Comments
: Any comments relating to the specimen lot's identification. Enter "Taxonomy verified." or "Taxonomy updated." in this field if you are simply updating the specimen's currently accepted name, but not physically/critically evaluating the specimen's true taxonomic identity. To be clear:
    - "Taxonomy updated." refers to new identifications that alter existing taxonomy, e.g. when a species is moved to a new genus, but the specimen was not physically examined by the identifier(s).
    - "Taxonomy verified." refers to repeat identifications that verify existing/historic identifications in the database, e.g. no taxonomic change is made to indicate the existing identification remains valid.
    
{% include figure image_path="/assets/images/catalogue_identification2.png" alt="screenshot of the identification tab in the catalogue module" caption="Screenshot of the *Identifications (1)* tab in the Catalogue module. This example demonstrates a taxonomic verification applied to a type specimen record." %}

ID Reference
: A [bibliography record]({{ site.baseurl }}/documentation/bibliography/) related to the identification can be attached via this field. While providing this information for specimen identifications in the LACMIP stratigraphic collection is optional, it must be provided for all taxonomic updates and verifications added to type specimen records. Additionally, unlike in the *IP Publications* table on the *Invert. Paleo.* tab, the literature or resource entered into *ID Reference* does not have to refer to a specific LACMIP specimen lot by catalog or type number, just the relevant species being verified or updated. It is preferable to enter static/published references over dynamic/web-based resources in this field.

Filed As
: This field should be "Yes" wherever *Currently Accepted* is also "Yes" and "No" wherever *Currently Accepted* is also "No," **except** for the records of **type specimens with outdated taxonomy** (see [re-identifications]({{ site.baseurl }}/documentation/reidentify/) for more on this). *Filed As* describes how the specimen is physically organized (filed) in the collection. This is why types, which may have had their taxonomy updated since their initial publication, are not always filed with a currently accepted name.

Currently Accepted
: This field should be "Yes" for any identification attaching a current taxonomic name, and "No" for invalid taxonomy as well as legacy identifications. Only one identification can have a value of "Yes" for *Currently Accepted*, so even if a legacy identification is taxonomically valid, you need to enter "No" for this field.

## Relationships tab

{% include figure image_path="/assets/images/catalogue_relationships.png" alt="screenshot of the relationships tab in the catalogue module" caption="Screenshot of the *Relationships* tab of the Catalogue module." %}

This tab allows you to associate catalog records, for example, when a bivalve and gastropod are preserved on the same rock and cataloged separately. The workflow used to do this can be found [here]({{ site.baseurl }}/documentation/relationships/).

Associating records using the *Relationships* tab is especially important for specimens filed in LACMIP's taxonomic collection; if this information is not recorded, these specimens may be nearly impossible to relocate.

## Location tab

{% include figure image_path="/assets/images/catalogue_location.png" alt="screenshot of the location tab in the catalogue module" caption="Screenshot of the *Location* tab of the Catalogue module." %}

LACMIP is still exploring how to use the *Location* tab, which is designed to track physical specimen movement. See the [Locations]({{ site.baseurl }}/documentation/locations/) module for an overview of the records you attach to this tab. Fields on this tab are...

Current Location
: Attach a [Locations]({{ site.baseurl }}/documentation/locations/) record here to indicate the current physical location of a specimen. Data from the Cretaceous inventory has been imported into EMu to auto-fill this field, although this data may not be up-to-date in all cases.

Movement metadata
: Fields like *Authorized By*, *Date Moved*, and *Reason* provide space to document metadata about specimen movement. LACMIP has not yet considered how to best use these fields.

Permanent Location
: Attach a [Locations]({{ site.baseurl }}/documentation/locations/) record here to indicate where a specimen should permanently be located, e.g. if the specimen is missing the *Current Location* is just "Carson Warehouse" and then *Permanent Location* records where the specimen ought to be. Data from the Cretaceous inventory has been imported into EMu to auto-fill this field, although this data may not be up-to-date in all cases.

Temporary Location
: Attach a [Locations]({{ site.baseurl }}/documentation/locations/) record here to indicate a temporary physical location of a specimen.

Independently Movable
: This field is a yes/no box to indicate whether or not a specimen can be independently moved. LACMIP does not currently have a use case for this box being checked "no."

Data in the fields above is tracked in the *Movement History* table. Please note that you cannot delete rows from this table, so if you enter and save a location accidentally, you cannot then delete it from the *Movement History* table. In practice, this is fine and you shouldn't worry about a "messy" entry.

## Registrar tab

The *Registrar* tab contains information about the provenance and disposition of the physical specimen(s) and is maintained by the Museum registrar. It is not visible to LACMIP student permission groups. Please do not edit fields on this tab.

## Multimedia tab

{% include figure image_path="/assets/images/catalogue_multimedia.png" alt="screenshot of the multimedia tab in the catalogue module" caption="Screenshot of the *Multimedia* tab of the Catalogue module." %}

If a specimen has been imaged, the image should be attached to the catalogue record and visible as an attachment on the *Multimedia* tab. In the screenshot above, you can see that the metadata from the [multimedia record]({{ site.baseurl }}/documentation/multimedia/) appears in the sidebar of this tab. Double-clicking on an image will open it in a larger viewer. Clicking on the green plus sign allows you to attach additional multimedia records.

## Admin tab

{% include figure image_path="/assets/images/catalogue_admin.png" alt="screenshot of the admin tab in the catalogue module" caption="Screenshot of the *Admin* tab of the Catalogue module, highlighting provenance and GUID data." %}

The *Admin* tab contains information about the record's digital provenance and edit history. This can be a useful way to check when and by whom a record was created or most recently modified. This tab is also where the record's GUID, or Global Unique Identifier, is stored. For catalogue records this is a critical identifier that gets published with the specimen occurrence data and ensures users can trace the data back to its source (i.e. the catalogue record at LACMIP).

The *Admin* tab is not visible to LACMIP student permission groups.

## Security tab

{% include figure image_path="/assets/images/catalogue_security.png" alt="screenshot of the security tab in the catalogue module" caption="Screenshot of the *Security* tab of the Catalogue module." %}

The only field you need to be concerned with on the *Security* tab is *Publish on Internet*, which should be check "Yes" for the majority of catalogue records but "No" for any records that should not be shared via biodiversity aggregators (e.g. iDigBio or GBIF; for more see [Publishing Data]({{ site.baseurl }}/documentation/ipt/)). A record should be marked "No" either because the specimen or its data are questionable, or as part of a research moratorium pending publication. Specific examples include but are not limited to:
- records where the specimen disposition is "missing"
- records where the specimen disposition is "discarded"
- records of type specimens of an unpublished new species
- records representing unsorted fossils
- records that may have been incorrectly catalogued

By default, EMu checks "Yes" for the *Publish on Internet* field, and also sets this as the default for searching catalogue records. If you feel that a record should not be made public, please go to this tab and check "No."

## Auxiliary tab

Only one field (*Aux. Rem 1*) on this tab is used, storing the *SpecIRN* value for catalogue records migrated from Access.
