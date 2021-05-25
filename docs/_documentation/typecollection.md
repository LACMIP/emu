---
title: Type Collection
navcat: Workflows
tags: cataloging
toc_sticky: true
last_modified_at: 2021-03-22
---

This documentation was created for the IP & Malacology Type Collection Renovation & Digitization project supported by [IMLS # MA-30-18-0335-18](https://www.imls.gov/grants/awarded/ma-30-18-0335-18-0), 2019-2021.

# Introduction

## What is a "type"?

Type specimens, or "types", are the physical, name-bearing vouchers for new taxa. They are retained in a specially designated "type collection" so researchers can reexamine them. Rules regarding types and their classification are maintained by the [ICZN](https://www.iczn.org/outreach/faqs/). Because types often represent new species, they include some of the museum's most intellectually valuable specimens and must be handled with extreme care.

 ~ | *Before accessing the type collection, review the following:*
   --- | ---
   ⚠️ | **Open drawers slowly and cautiously.** Be aware that these cabinets do not have drawer stoppers. In other words, if you pull too far, the drawer may fall out. As a precaution, always pull out the drawer immediately below the one you wish to access about halfway.
   ⚠️ | **Always ask for help when moving drawers around.** They may be much heavier than they appear. 
   ⚠️ | **If type specimens are damaged or disassociated from their labels, alert the collections staff immediately.** Never move specimens or labels between boxes, or reorganize the boxes within their drawers unless directed to do so.
   🔑 | All type specimens must be returned to their appropriate drawers and cabinets at the end of your shift. Similarly, the type room is a communal workspace (shared with Malacology) and should be kept tidy.
   🔑 | Please do not invite visitors into the type collection without permission from the Collections Manager or Curator.
   🚫 | Water is allowed in the type room, but should be kept away from specimens and equiment at all times. Please store/consume food and other beverages elsewhere.
   ❓ | Always ask questions when you're not sure what to do!

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

The workflow used to edit and quality control (QC) type specimen records is outlined below. To enlarge screenshots, right click and open them in a new tab or window.

## I. Search for a specimen

Search for type specimens using their LACMIP type numbers. These numbers are always labelled on specimens in bright red, yellow, or blue paint (_never_ white paint or stickers). If you are unsure whether a number represents a type number, consult [these keys]({{ site.baseurl }}/documentation/typecollection/#number-keys).

{% include figure image_path="/assets/images/catalogue_LACMIPtypeno.png" alt="example LACMIP Type No." caption="LACMIP type numbers are indicated by bright red, yellow, or blue paint. Red = holotypes, syntypes, lectotypes; Yellow = paratypes, paralectotypes; Blue = hypotypes (figured or unfigured specimens)." %}

{% include figure image_path="/assets/images/catalogue_typesearch.png" alt="screenshot of the Invert. Paleo. tab's search form in the Catalogue module" caption="Screenshot of the *Invert. Paleo.* tab's search form in the Catalogue module." %}

 *Step* | *On the search form...*
   --- | ---
   1 | In *LACMIP Type No.*, enter the type number. 
   2 | Select the binoculars icon to execute the query.
   3 | If no records are returned using *LACMIP Type No.*, but the catalog number is indicated on an old specimen label in the box, use it to search for the specimen in *Cat. No.* In [this example](https://lacmip.github.io/emu/assets/images/cataloging_edits.jpg), you would search for "23225.291" or "31458.1".
   4 | If no records are returned and you are certain there were no typos in your searches, ask the collections staff for help.

Once you get comfortable with EMu, tips on searching for records can be found [here]({{ site.baseurl }}/documentation/modes/#search-mode).
{: .notice--warning}
   
## II. Assess the catalog record

{% include figure image_path="/assets/images/catalogue_invertpaleo_typeunedited.png" alt="screenshot of the Invert. Paleo. tab's search form in the Catalogue module" caption="Screenshot of what a typical, unedited catalog record for a type specimen looks like." %}

For each type specimen, assess the information on its catalog record according to guidance outlined below. You should only be concerned with information on the Invert. Paleo. tab and, in the uncommon event that several specimens are stuck together, the Relationships tab. 

 *Field* | *On the Invert. Paleo. tab...*
   --- | ---
   *Locality* & *Cat. No.* | Verify that the LACMIP locality and catalog numbers listed on the catalog record match the locality number painted on the specimen in white paint, as well as what's on the specimen's old label(s) in its box. (Reminder: This is what a [locality number]({{ site.baseurl }}/assets/images/catalogue_localitynumbers.jpg) looks like and this is what a [catalog number]({{ site.baseurl }}/assets/images/cataloging_edits.jpg) looks like.) You may need to open the corresponding Sites record to compare (use the blue arrow to open it). While mismatches are uncommon, immediately alert the collections staff if you find one.
   *Lot Count* | Verify the number of specimens in the lot that have the same type number. In the type collection, this value is **typically "1"**, but occasionally there will be more than one fossil (or piece of fossil) with the same type number; in either case, update the lot count to reflect the true number of specimens. Refer to the [guidelines for counting]({{ site.baseurl }}/documentation/digitizing/#counting) and ask for help if you're still unsure. Do not count synthetic objects, like rubber peels, that may also be in the box.
   *Disposition* | Verify the physical state of the specimen lot. For the vast majority of lots, you will verify that they are in the collection by choosing **"in collection"**. However, if you encounter an empty box, a specimen may be "missing" or "on loan", and *Disposition* should be updated accordingly. **If the specimen is missing**, transcribe any relevant notes you find in the box into *Lot Remarks*, [for example]({{ site.baseurl }}/assets/images/catalogue_missing.png), "G.S., 9/1971, Missing". Likewise, **if the specimen is on loan**, transcribe any relevant information at your disposal into *Lot Remarks* in [this format]({{ site.baseurl }}/assets/images/catalogue_loan.png): "On loan to [name], [affiliation] (YYYY-MM-DD) (email)". Ask the collections staff if the correct disposition is not readily apparent.
   *P/CP* | Refers to "part" (P) and counterpart" (CP) and is typically used for compression fossils and concretions. If both parts (halves) are present, check this box and make sure *Lot Count* is updated accordingly.
   *Alternative Numbers* | <img src="{{ site.baseurl }}/assets/images/catalogue_alternativenumbers.png" alt="" width="500"/>{: .align-center} Record [legacy catalog numbers]({{ site.baseurl }}/assets/images/catalogue_alternativenumbersexample.jpg) assigned by another institution or the collector in this table. ***Inst. Code*** typically refers to an institution, like "UCLA", "CIT", or "CSUN". Use the lookup list button when entering an *Inst Code* to validate your entry. If you are trying to add a new institution code, please ask for assistance. Occasionally, the number might be a collector number. In that case, enter "collector number" in this field. ***Inst. Number*** can either refer to a number assigned by an institution (such as UCLA) or a collector (such as W. D. Pierce). In the case of a collector, the number should be formatted as capitalized name and number (e.g. "PIERCE 32a"). *Do not record old locality numbers in this table*, which are typically found on circular stickers in the type collection. Use the [number keys appendix]({{ site.baseurl }}/documentation/modes/#numbers-keys) to guide you.

{% include figure image_path="/assets/images/catalogue_alternativenumbersexample.jpg" alt="Example of an old catalog number to be entered in *Alternative Numbers*" caption="Example of an old catalog number to be entered in *Alternative Numbers*. In general, UCLA catalog numbers will look very similar to the one illustrated above (i.e. handwritten on a white rectangular label and adhered to the specimen)." %}

If you are unsure how to record a number, take a quick photo of the specimen (with the number visible), as well as any relevant specimen labels, and send them to the IP collections staff in Google Chat.
{: .notice--warning}

 *Field* | *On the Invert. Paleo. tab...*
   --- | ---
    *Type Status* | Refers to the most important status conferred upon a type specimen. In the unlikely event that this value is incorrect, use the dropdown and select the most important kind of type listed the *IP Pubications* table: **1, most important:** holotypes, syntypes, lectotypes, neotypes; **2:** paratypes, paralectotypes, allotypes; and **3, least important:** hypotypes, figured and unfigured.
    *Collection* | Value should always be "TYPE".
    *Project* | If blank, choose "IMLS".
    *Original Nature* | ***Ignore this field.*** The default value is "body fossil". This information will be updated at a later time.
    *Anatomy* | ***Ignore this field.*** The default value is "body". This information will be updated at a later time.
    *Lot Remarks* | Only enter information in this field if you find a lot with a [missing]({{ site.baseurl }}/assets/images/catalogue_missing.png) specimen or a specimen [on loan]({{ site.baseurl }}/assets/images/catalogue_loan.png). See *Disposition* for more information on missing and loaned lots.
    
## III. Verify publication history

{% include figure image_path="/assets/images/catalogue_ippublications.png" alt="screenshot of the Invert. Paleo. tab's search form in the Catalogue module" caption="Screenshot highlighting the *IP Publications* table on the Invert. Paleo. tab. More rows in this table will become visible if you stretch the window, as in the image above." %}

Specimens are designated as types if they are cited in publications, and this information is tracked in the *IP Publications* table.

 *Field* | *In the IP Publications table...*
   --- | ---
    *Publication* | **If a publication is already listed in the table**, verify the information in the *Pages*, *Fig.*, and *Type* fields using a copy of the book or paper. LACMIP maintains a collection of reprints for this purpose. If you need to search for a digital copy, please [consult the appendix]({{ site.baseurl }}/documentation/typecollection/#gathering-literature) **If a publication is missing from the *IP Publications* table**, it needs to be attached using the Bibliography module. To do so, search for the publication by typing in a few key words from its title or one or a few lastnames from the author list and press tab or select the green ➕ button. If an entry for this publication already exists in the Bibliography module, it may automatically attach itself to the row. Verify that the correct record was retrieved. It is also possible that you will be presented with several options. In this case, [locate the correct record]({{ site.baseurl }}/assets/images/bibliography_ippublications.png) and attach it to *Publications* using the green ➕ button. If you are certain the correct Bibliography record does not exists yet, you will need to create a new one. **To create a new Bibliography record,** consult the documentation for the [Bibliography module]({{ site.baseurl }}/documentation/bibliography/).

If you need to create a new Bibliography record, search for an existing one from the same journal and use it as a template for the new record using ditto. The [gathering literature]({{ site.baseurl }}/documentation/bibliography/#gathering-literature) section of the appendix outlines where and how to add digital literature to the LACMIP reprint library. 
{: .notice--warning}

 *Field* | *In the IP Publications table...*
   --- | ---
    *Pages* | Enter the page number(s) where the specimen is described. Do not enter "p.", "pg.", etc. before the number(s).
    *Fig* | Enter the plate and figure number(s) separated by a colon. For example: "pl. 1: fig. 1-3". If a specimen is figured on multiple plates, separate these entries with a semicolon. For example, "pl. 1: fig. 1-5; pl. 4: fig. 3b, 3c". If the figure is unnumbered, enter "fig. unnumbered". If the specimen is unfigured, enter "unfigured". This field can be stretched horizontally if needed.
    *Type* | Indicate what kind of type the specimen is according to the publication. For specimens cited in theses, dissertations, and historic manuscripts, enter "Unpublished". The first letter should be uppercase, e.g. "Holotype".

Publications in this table should be listed chronologically with the **oldest (first) publication** appearing **in the top row**. If needed, click and drag to reorder these entries. You may wish to print this [formatting cheatsheet]({{ site.baseurl }}/assets/images/catalogue_ippublicationsformatting.png) for values in *Page* and *Fig*.
{: .notice--warning}

More on how LACMIP types are cited and the history of these numbers can be found [here]({{ site.baseurl }}/documentation/citing/).
{: .notice--warning}

## IV. Relate associated specimens

{% include figure image_path="/assets/images/catalogue_relationships.png" alt="screenshot of the Relationships tab in the Catalogue module" caption="Screenshot of the Relationships tab in the Catalogue module. Records for specimens that are physically stuck together, but are cataloged separately, need to be associated using this tab." %}

Occasionally, you will encounter specimens that are physically stuck together but cataloged separately (they should also have different type numbers). In this case, their respective catalog records need to be associated using the Relationships tab. The general workflow for using the Relationships tab can be found [here]({{ site.baseurl }}/documentation/cataloging/#relationships-tab). This workflow is also demonstrated in this video:
{% include video id="417827299" provider="vimeo" %}

## V. Note special conditions 

{% include figure image_path="/assets/images/catalogue_condition_oversize.png" alt="screenshot of the Condition tab in the Catalogue module" caption="Screenshot of the Condition tab in the Catalogue module." %}

### Oversized Lots
Specimens that do not fit in one of our standard box sizes are considered oversized. In this situation, a special mount/box will need to be created for it at a later time. Please indicate this information by completing the following fields on the Condition tab:

*Field* | *On the Condition tab...*
   --- | ---
    *Condition Status* | Select "**Unstable; may require special mount.**"
    *Date Checked* | Select today's date.
    *Checked By* | Attach your Parties record. 
    *Condition Details* | "**Oversized lot.**"
    
### Damaged Lots    
Specimens that are clearly damaged or deteriortating should be noted. Please indicate this information by completing the following fields on the Condition tab:
    
 *Field* | *On the Condition tab...*
   --- | ---
    *Condition Status* | Select "**May require treatment.**"
    *Date Checked* | Select today's date.
    *Checked By* | Attach your Parties record. 
    *Condition Details* | Briefly describe the problem, e.g. "Specimen is deteriorating. Consolidation required." or "Number painted on specimen should be removed and corrected. It should be 12760."
    
    

## VI. Locate specimens

The final step is to assign (or reassign) the physical location data to specimen lots.

On any given day, you'll likely be working with specimens in only one or two drawers. At the end of your shift, or if you finish working on a drawer mid-shift--whichever comes first--you'll need to update the physical location data for all the lots you worked on.

To update locations for multiple records at once:

 *Step* | *In the Catalogue module...*
   --- | ---
    1 | Navigate to the search form (*File > New Search*). 
    2 | On the search form, navigate to the Admin tab.
    3 | Enter your name in *Modified By*, the date in *Modification Date*, and execute the search.
    4 | Review the results in List view.
    5 | Hold shift to select all records from the same drawer. ⚠️**Critical: Make sure you're only selecting lots that came from the same drawer.**
    6 | Navigate: *Tools > Relocate > Selected Records*
    7 | In the Location Update window, click on the green ➕ to open the Locations module.
    8 | In the Locations module, enter "Type Room" in *Level 3*.
    9 | In the Locations module, use the lookup list buttons for *Level 4* and *Level 5* to enter the cabinet and drawer. [(Example.)]({{ site.baseurl }}/assets/images/catalogue_locationupdate_typeexample1.png)
    10 | Execute the search and open the record to verify the correct one was returned.
    11 | Attach this record to the Location Update window with the green ➕.
    12 | In the Location Update window, attach your Parties record to *Requested By*, *Released By*, and *Accepted By* and enter the date in *Date Moved*. [(Example.)]({{ site.baseurl }}/assets/images/catalogue_locationupdate_typeexample2.png)
    13 | Select *Update*.
    14 | Review the updated records to check for errors.
    
Location history cannot be deleted. It is therefore very important that you take care when selecting records to be batch relocated.
{: .notice--warning}

# Appendices

## Gathering literature

### Find the publication

When searching for digital publications it can be useful to check the resources listed below. They are listed from more general purpose to more specific:

1. [Google Scholar](https://scholar.google.com/)

2. [IMLS Type Publications folder](https://drive.google.com/drive/folders/1Ej6RF7llwTXr4qvrzZv9XuWY222T1Ahy?usp=sharing)

3. [Biodiversity Heritage Library](https://www.biodiversitylibrary.org/)

4. [PBDB](https://paleobiodb.org/#/)

If you cannot readily find the publication you're looking for, send the collections staff a request via Google Chat.

## Number keys

### Type numbers

Colorized numbers typically represent LACMIP Type Numbers:

| *Type* | Color | 
| ---------------- | ------ |
| Holotype/Syntype | Red    | [example]({{ site.baseurl }}/assets/images/imls_numbers_typered.jpg) | 
| Paratype         | Yellow | [example]({{ site.baseurl }}/assets/images/imls_numbers_typeyellow.jpg) |
| Hypotype/Figured | Blue   | [example]({{ site.baseurl }}/assets/images/imls_numbers_typeblue.jpg) |


### Alternative numbers
Identifiers used by institutions/collections that previously owned specimens in the LACMIP collections are recorded in the *Alternative Numbers* table. Only specimen numbers, **not locality numbers**, should be added to this table. (Old locality numbers are recorded elsewhere.) Use this guide to help you determine if a number should be added to this table.

{% include figure image_path="/assets/images/catalogue_alternativenumbers.png" alt="screenshot of the Alternative Numbers table in the Catalogue module" caption="Screenshot of the Alternative Numbers table in the Catalogue module." %}

| *Inst. Code.* | Number Style | Record in *Alt. Numbers*? |
| - | - | - |
| **UCLA**         | **white rectangle**           | ✔️**YES** | [example]({{ site.baseurl }}/assets/images/imls_numbers_uclacatalog.jpg) |
| **CIT**          | **check label/box**           | ✔️**YES** | [example]({{ site.baseurl }}/assets/images/imls_numbers_citcatalog.jpg) |   
| **collector number** | **various/unique**        | ✔️**YES** | [example]({{ site.baseurl }}/assets/images/imls_numbers_collectornumber.jpg) |
| CIT              | gold dot                      | ⛔locality | [example]({{ site.baseurl }}/assets/images/imls_numbers_citlocality.jpg) |
| CSUN             | red dot                       | ⛔locality | [example]({{ site.baseurl }}/assets/images/imls_numbers_csunlocality.jpg) |
| LACMIP           | white paint                   | ⛔locality | [example]({{ site.baseurl }}/assets/images/imls_numbers_lacmiplocality.jpg) |
| SDSU             | red paint                     | ⛔locality, looks like type # | [example]({{ site.baseurl }}/assets/images/imls_numbers_sdsulocality.jpg) |
| UCLA             | green dot                     | ⛔locality | [example]({{ site.baseurl }}/assets/images/imls_numbers_uclalocality.jpg) |
| USGS             | various                       | ⛔locality | [example]({{ site.baseurl }}/assets/images/imls_numbers_usgslocality.jpg) |

One way to check whether a number is an old locality number is by clicking the blue arrow button next to the *Locality*. If your number appears in the *Institution Number* table, you have a locality number. In that case, do not record it in *Alternative Numbers*.

If you're not sure what a number represents, take a photo of it and send it to collections staff in the Google Chat or via email.
{: .notice--warning}
