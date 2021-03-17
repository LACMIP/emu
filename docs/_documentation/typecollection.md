---
title: Type Collection
navcat: Workflows
tags: cataloging
last_modified_at: 2021-03-15
---

The following documentation was created for the LACMIP Type Collection Renovation & Digitization project funded by the Institute of Museum & Library Services [(IMLS Award # MA-10-19-0223-19)](https://www.imls.gov/grants/awarded/ma-10-19-0223-19-0).

# Introduction

## What is a "type"?

Type specimens, or "types", are the physical, name-bearing vouchers for new species, genera, etc. They are therefore retained in a specially designated "type collection" so researchers can reexamine them to assess their taxonomic validity. Therefore, types are some museum's most intellectually valuable specimens and must be handled with extreme care.

 *!* | *Before accessing specimens in the type collection, review the following:*
   --- | ---
   ⚠️ | **Open drawers slowly and cautiously.** Be aware that these cabinets _do not_ have drawer stoppers. In other words, if you pull to hard, the drawer may fall out. As a precaution, always pull out the drawer immediately below the one you wish to access about halfway; it will act as an emergency "stopper" should you pull out the upper tray too far.
   ⚠️ | **Always ask for help when moving drawers around.** They may be much heavier than they appear. 
   ⚠️ | **If type specimens are damaged or disassociated from their labels, alert the collections staff immediately.** Never move specimens or labels between boxes, or reorganize the boxes within their drawers unless directed to do so.
   🔑 | All type specimens must be returned to their appropriate drawer(s)/cabinet(s) at the end of your shift. Similarly, the type room is a communal workspace (shared with Malacology) and should be kept tidy.
   🔑 | Please do not invite visitors into the type collection without permission from the Collections Manager or Curator.
   🚫 | Water is allowed in the type room, but should be kept away from specimens and equiment at all times. Please store/consume food and other beverages elsewhere.
   ❓ | Always ask questions when you're unsure what to do!

## What is "taxonomy"?

In the biological sense, taxonomy refers to the identification and interpretation of organisms within natural groups. While you will not be entering or editing specimen identifications or taxonomy in EMu, taxonomy forms the foundation upon which the type collection is organized, and it is therefore important that you familiarize yourself with the basic concepts of taxonomy and binomial nomenclature by reviewing [this article](https://www.digitalatlasofancientlife.org/learn/systematics/taxonomy/) and/or the following video. The ICNZ also provides helpful [definitions](https://www.iczn.org/outreach/faqs/#faq-1).
{% include video id="12XO8vYqBsA" provider="youtube" %}

## QC/Editing vs. Cataloging

Most of the specimens in the type collection are cataloged, i.e. they already have a catalog number, which is a unique, human-readable identifier for a specimen lot to be cited when specimens are referenced in published research. 

Instead of cataloging, you will be editing and updating--or "QC'ing" (quality controlling)--existing catalog records with missing information.

Before editing any catalog records for type specimens, please *thoroughly* review our comprehensive documentation for the [Catalogue module]({{ site.baseurl }}/documentation/catalogue/), as well as all steps below outlined below.

**Interns and volunteers will rarely catalog specimens in the type collection**. As a point of diambiguation, true "cataloging" refers to the creation of _new_ catalog records and is only needed when new types are received from researchers. This should only be done with guidance from the Collections Manager. LACMIP maintains a separate workflow for [cataloging]({{ site.baseurl }}/documentation/cataloging/).
{: .notice--warning}

# Type Collection QC Workflow

The workflow below is used to edit and quality control (QC) type specimen records is outlined below. To enlarge screenshots, right click and open them in a new tab or window.

## Search for a type specimen

Search for type specimens using their LACMIP type numbers. These numbers are always labelled on specimens in bright red, yellow, or blue paint (_never_ white paint or stickers). If you are unsure whether a number represents a type number, consult the collections staff.

{% include figure image_path="/assets/images/catalogue_LACMIPtypeno.png" alt="example LACMIP Type No." caption="LACMIP type numbers are indicated by bright red, yellow, or blue paint. Red = holotypes, syntypes, lectotypes; Yellow = paratypes, paralectotypes; Blue = hypotypes (figured or unfigured specimens)." %}

{% include figure image_path="/assets/images/catalogue_typesearch.png" alt="screenshot of the Invert. Paleo. tab's search form in the Catalogue module" caption="Screenshot of the *Invert. Paleo.* tab's search form in the Catalogue module." %}

 *Step* | *On the search form...*
   --- | ---
   1 | In *LACMIP Type No.*, enter the type number. 
   2 | Select the binoculars icon to execute the query.
   3 | If no records are returned and an old [2000s-style specimen label]((https://lacmip.github.io/emu/assets/images/cataloging_edits.jpg)) is present in the box, search for the specimen using the catalog number in *Cat. No.*. In this example, you would search for "31458.1".
   4 | If no records are returned and you are certain there were no typos in your searches, ask the collections staff for help.

Once you get comfortable with EMu, tips on searching for records can be found [here]({{ site.baseurl }}/documentation/modes/#search-mode).
{: .notice--warning}
   
## Assess the catalog record

{% include figure image_path="/assets/images/catalogue_invertpaleo_typeunedited.png" alt="screenshot of the Invert. Paleo. tab's search form in the Catalogue module" caption="Screenshot of what a typical, unedited catalog record for a type specimen looks like." %}

For each type specimen, assess the information on its catalog record according to guidance outlined below. You should only be concerned with information on the Invert. Paleo. tab and, in the uncommon event that several specimens are stuck together, the Relationships tab. 

 *Field* | *On the Invert. Paleo. tab...*
   --- | ---
   *Locality* & *Cat. No.* | Verify that the LACMIP locality and catalog numbers listed on the catalog record match the locality number painted on the specimen in white paint, as well as what's on the specimen's old label(s) in its box. (Reminder: This is what a [locality number](https://lacmip.github.io/emu/assets/images/catalogue_localitynumbers.jpg) looks like and this is what a [catalog number](https://lacmip.github.io/emu/assets/images/cataloging_edits.jpg) looks like.) You may need to open the corresponding Sites record (use the blue arrow to open it) to compare. While mismatches are uncommon, immediately alert the collections staff if you find one.
   *Lot Count* | Refers to the number of individual specimens with the same type number. In the type collection, this value is typically "1". However, occasionally there will be more than one fossil with the same type number in a lot. In that case, update the lot count to reflect the true number of specimens. Refer to the [guidelines for counting]({{ site.baseurl }}/documentation/digitizing/#counting) and ask for help if you're still unsure. Do not count synthetic objects (like rubber peels) that may be left in the box.
   *Disposition* | <img src="{{ site.baseurl }}/assets/images/catalogue_lotremarks_loan.png" alt="" width="500"/>{: .align-center} A dropdown menu with options to note the physical state of a specimen lot. For the vast majority of specimens, you will verify that they are in the collection by choosing "in collection". If you encounter an empty box, a specimen may be missing or on loan, and the disposition should be changed to indicate this. If the specimen is missing, transcribe any relevant notes in the box into *Lot Remarks* (for example, "MISSING 02/17/70 ECW). Likewise, if a specimen is on loan, transcribe any relevant infomration at your disposal into the *Lot Remarks* in this format: "On loan to [name], [affiliation] (YYYY-MM-DD) (email). Verify with the Collections Manager if the correct disposition is not readily apparent.
   *P/CP* | Refers to "part" and counterpart" and is typically used for compression fossils and concretions. If both parts are presents, check this box and make sure the *Lot Count* is also updated accordingly.
   *Alternative Numbers* | <img src="{{ site.baseurl }}/assets/images/catalogue_alternativenumbers.png" alt="" width="500"/>{: .align-center} Used to record legacy catalog numbers assigned by another institution or the collector. *Inst. Code* typically refers to an institution, like "UCLA", "CIT", or "CSUN". Use the lookup list button when entering an *Inst Code* to validate your entry. If you are trying to add a new institution code, please ask for assistance. Occasionally, the number might be a collector number. In that case, enter "collector number" in this field. *Inst. Number* can either refer to a number assigned by an institution (such as UCLA) or a collector (such as Pierce). In the case of a collector, the number should be formatted as capitalized name and number (e.g. 'PIERCE 32a'). Do not record old locality numbers (typically on circular stickers) in this field. Additional explanation of *Alternative Numbers* is provided [here]({{ site.baseurl }}/documentation/catalogue/#invert-paleo-tab)

{% include figure image_path="/assets/images/catalogue_alternativenumbersexample.jpg" alt="Example of an old catalog number to be entered in *Alternative Numbers*" caption="Example of an old catalog number to be entered in *Alternative Numbers*. In general, UCLA catalog numbers will look very similar to the one illustrated above (i.e. handwritten on a white rectangular label and adhered to the specimen)." %}

If you are unsure how to record a potential alternative number, take a quick photo of the specimen (with the number visible), as well as any relevant specimen labels, and send them to the IP collections staff in Google chat.
{: .notice--warning}

 *Field* | *On the Invert. Paleo. tab...*
   --- | ---
    *Type Status* | Refers to the most important status conferred upon a given type specimen. (See "[What kinds of types are there?](https://www.iczn.org/outreach/faqs/#faq-4)" according to the ICZN.)  Historically, hypotypes/figured specimens (=blue type numbers) were also included in the LAMCIP type collection. For these specimens, always choose "hypotype".
    *Collection* | Value should always be "TYPE".
    *Project* | If blank, choose "IMLS".
    *Original Nature* | Ignore this field. The default value is "body fossil". This information will be updated at a later time.
    *Anatomy* | Ignore this field. The default value is "shell(s)". This information will be updated in bulk.
    
## IP Publications

    
    *IP Publications* | <img src="{{ site.baseurl }}/assets/images/catalogue_IPpublications.png" alt="" width="500"/>{: .align-center} Refer to the explanation for [IP Publications]({{ site.baseurl }}/documentation/catalogue/#invert-paleo-tab) for the most updated, authoritative information on how to complete this table. If a new Bibliography record needs to be attached or created, consult the [Bibliography](#bibliography) workflow. 



`Pages, Fig. & Type` : data about where a specimen waas described in the cited paper. 
    - `Pages` : format with only the page number. Do not enter `p.`, `pg.`, ect. 
    - `Fig` : Enter the plate and/or figure number(s) seperated by a colon. See following examples: 
      + Specimen not figured: `unfigured`
      + Only plate: `pl. 3`
      + Only figure: `fig. 1`
      + Figure with range: `fig. 1A-B`
      + Multiple figures: `fig. 1, 3, 5-7`
      + Plate and only one figure: `pl. 3: fig. 15`
      + Plate and range of figures: `pl. 3: fig 9-15`
      + Plate and sequence of figures listed: `pl. 3: fig. 7, 12, 24`
      + Multiple plates: `pl. 3: fig. 7, 12, 24; pl.4: fig.8`
    - `Type`: open text field for kind of type 
      + Capitalize first letter


### Identification (1) tab
Below is an example of when the taxon of a specimen in known and needs to be entered. This only needs to be done if the genus nad species listed on a type specimen's record is not already entered in the `Identification List` nested table. 

If attempting to add a taxon to a catalog record, please ask for guidance.

A complete overview of the fields in the [Identification (1) tab](https://lacmip.github.io/emu/documentation/catalogue/#identification-1-tab) exists on the LACMIP EMu Handbook under the Catalogue page. Below are the fields that will be primairly used for cataloging type records. 

![img](https://lh6.googleusercontent.com/Zj6wDB0ph_2twEn60XdpzgmXW9Cura8lZfiNF_qElfNGgeisZIwrM1zcEzebOrewdLHg7xcmOunvI3SKP4CMde0Oi5S7wL-rjr3l4wtTacL3aEfVS7vawcGHLQS5rbFdYGBulYhi)

1. `Taxon` : attached record from the Taxonomy module that is currently selected from `Identification List`. 
    - If known, type the genus and species into and box and search for the taxon by clicking the blue button.
    - If the correct taxon is not available add the following text to the `Comments` open text box:
    > originally identified as [taxon]; taxonomy for this name does not exist in EMu (yet)
    >
2. `Identified By` : lookup list of full name(s) of person(s) who made this identification. 
    - Should only be filled out if label or publication explicitly states who identified (not collected) specimen. 
    - Generally formatted as `[first initial]. [surname]` though occasionally as `[first name] [surname]`. 
    - `Date Identified` : should only be filled out if date for identification is provided. Can be as granular as a day or a year. 
    - `Identification List` : tabel displaying the different taxa associated with a specimen
      + `Filed As` and `Currently Accepted` are radio buttons that take special meaning for type records. If attaching a new taxonomy, please consult collection manager for guidance. 
      + `*` : Clicking this button will add a new row in the nested table so more taxon records can be added. 

### Location tab

Locations for each specimen are recorded in EMu based on which cabinet and drawer they reside in. 

![screenshot of the location tab in the catalogue module](https://lacmip.github.io/emu/assets/images/catalogue_location.png)

1. `Current`  : type in `Cabinet [#] Drawer [#]` of the cabinet, drawer pair and press 'Tab' or the blue arrow to populate the field. 
   - If nothing populated, ask Daniel for help.
2. `Authorized By:` : type in `Daniel Markbreiter` and the blue arrow/tab.
3. `Moved By` : enter your full name and the blue arrow/tab.
4. `Inventoried  : enter your full name and the blue arrow/tab.

### Condition tab

![img](https://lh6.googleusercontent.com/9X6hV6Bu6yNbNpZbhlw3UIqKtoMqmTv7_7ldYMCIMctmYVf8HDAWDf9BSiOMD5xv2Q_1d7lBQDYPluJF_KbcljgANzJ98n-7gtW9qH_PpW6pUpnLqQTutWKAkWQS6hyn1O8xb5kP)

This tab is intended for specimens that will require special attention by the volunteers who rehouse the type specimens. 

1. `Condition Status` : choose 'The object is fragile and requires treatment' if specimen is oversized and will require a special mount.

## Bibliography

Using the Bibliography module is typically only required when a catalogue record needs an additional entry to the `Publication` nested table. The easiest way to enter the Bibliography module to accomplish this is by clicking the plus sign button to the very right of the table. 

This IMLS bibliography workflow was adapted from the [Bibliography](https://lacmip.github.io/emu/documentation/bibliography/) page of the LACMIP EMu Handbook. Please consult this reference for an expanded explanation of the module. 

### Creating Bibliography records

This tab is where the bulk of the bibliographic information will need to be recorded. Please refer to the [Bibliography](https://lacmip.github.io/emu/documentation/bibliography/) page of the LACMIP EMu Handbook for a detailed list of fields and their definitions. 

**Below is list of required fields:**

If journal article: 

- `Title`
- `Journal`

If book: 

- `Book Title`

For all publication types: 

- `Author`
- `Pages` 
- `Year`

**Below is a list of required fields, if information is available**:

- `Year Letter`
- `Volume`
- `Publ. No.`
- `Series`
- `Editor`
- `DOI`

### Attaching a bibliography record

After a record is completed, click the `Attach to record` button (see below) in the top right of the application window in the tool bar. 

![image-20210314132842902](/Users/macbook/Library/Application Support/typora-user-images/image-20210314132842902.png)

Once attached, the bibliography record should show as an entry in the `Publication` table. 

### Adding PDFs to Google Drive

If a PDF of the publication is available for download, please include it in the [Type Publications](https://drive.google.com/drive/folders/1Ej6RF7llwTXr4qvrzZv9XuWY222T1Ahy?usp=sharing) directory of the `IMLS` Google Drive. If you do not have access to the linked Google Drive directory, please ask for access. 

#### Formatting PDF filenames

It is imperative that PDF filenames conform to the convention applied to the other PDF files in the `Type Publications` directory. These PDFs will eventually be uploaded as multimedia attachments to their associated EMu record. Incorrect formatting can cause errors when they are uploaded. 

**Single author**
```
[Surname], [First initial]. [Middle initial]. ([Year]) [Title]
```
**Two authors**
```
[Surname], [First initial]. [Middle initial]. & [Surname], [First initial]. [Middle initial]. ([Year]) [Title]
```
**Three to four authors**
```
[Last name], [First initial]. [Middle initial]., [Last name], [First initial]. [Middle initial] and [Last name], [First initial]. [Middle initial]. ([Year]) [Title]
```
**Five or more authors**
```
[Last name], [First initial]. [Middle initial]., et al ([Year]) [Title]
```
**Example**:
> Valentich-Scott, P., Powell, C., L., Lorenson, T. D. & Edwards, B. E. (2014) A new genus and species of Thyasiridae (Mollusca, Bivalvia) from deep-water, Beaufort Sea, northern Alaska.pdf

## Appendix

### Institutional Numbers

Institutional numbers are the old identifiers used by previous institutions/collections. They are added in the `Identification` tab in the `Invert Paleo` tab. 

There are both institutional locality and catalogue numbers. **Only catalogue numbers are added to the Indentification tab**. To verify that you have the correct number is by opening the locality record attached to the catalog record (clicking the blue button next to the `Locality` field). If you see your number under the `Institution Number` nested table, you have a locality number. 

#### Frequently encountered institution numbers

| Institution Code | Locality sticker color | Catalogue sticker               |
| ---------------- | ---------------------- | ------------------------------- |
| UCLA             | Green                  | White rectangular handwritten sticker |
| CIT              | Gold                   | -                               |
| CSUN             | Red                    | -                               |
| USGS             | -                      | On label                        |
| SDSU             | Red (painted)          | -                             |
| Collector Number | Unique | Unique |

##### UCLA

<ins>Institution catalogue number</ins>: The institution catalogue number will be written on a **white rectangular** label glued onto the specimen. 

<ins>Institution locality number</ins>: found on a circular **green** sticker on specimen. 

<img src="https://lh6.googleusercontent.com/-5BBn2wceTEZzl_aDvQa2pmIL6Ak27rn41O2ZNIoYJMrlbx5PQ1R7FjQEGzgH8qM9TWkCicd9p3BuwoNqpORuB8q7IWpnejfHdgSnfcenVtpKr_2AOwYdmzdJq7qBdruqdawK5xK" width="400"/> <img src="https://lh6.googleusercontent.com/3OBzjamYzWe22sbhoSnQuEgI8vPXsoYusZIvIyV1B69YC6XJKF_AOMDwFTRiVgyk3Bo9xPT29fAOC-kQKG6IMkETYf7r2aGSXGDFJvIFkgfoN7UVdwTbJSGPXa1FGGnQo4cyOaLQ" alt="photo of specimen label with UCLA locality number" width="200"/>



##### CIT

<ins>Institution catalogue number</ins>: typically CIT specimens do not have an associated CIT catalogue number. 

<ins>Institution locality number</ins>: found on a circular **gold** sticker on specimen. 

<img src="https://lh4.googleusercontent.com/e1-bZp2MdcMll3pBBELgRSyfRMc-r8amGX3AXZ0IH3fyIgFz1abz0AAgnXmJKDtWZJj3CSH5sclnZmXL4xxsvrAowKKEBl1T-LltMpvXenCheW2kTu62ck3xiGhKIYWvln-k_k9P" width="300"/>

##### CSUN

<ins>Institution catalogue number</ins>: typically CSUN specimens do not have an associated CSUN catalogue number. 

<ins>Institution locality number</ins>: found on a circular **gold** sticker on specimen. 

### Type color codes

Type specimens in the collection will either have painted numbers or typed labels with font colors correspondig to the kind of type specimen it is. Below is reference to the three colors of type numbers in the collection.

| Type             | Color  |
| ---------------- | ------ |
| Holotype/Syntype | Red    |
| Paratype         | Yellow |
| Hypotype/Figured | Blue   |

### Finding publications

Addind publications to a type catalogue record is the most critical part of cataloging for the IMLS project. When searching or publications it can be useful to check the resources listed below. They are listed in the order of general purpose to more specific. 

1. [Google Scholar](https://scholar.google.com/)

2. [IMLS Type Publications folder](https://drive.google.com/drive/folders/1Ej6RF7llwTXr4qvrzZv9XuWY222T1Ahy?usp=sharing)

3. [Biodiversity Heritage Library](https://www.biodiversitylibrary.org/)

4. [PBDB](https://paleobiodb.org/#/)
