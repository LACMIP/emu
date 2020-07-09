---
title: Cataloging
navcat: Workflows
tags: cataloging
last_modified_at: 2020-07-08
---

Cataloging (a.k.a. databasing) is a critical step in digitization, and the creation of accurate digital catalog records facilitates collection management and access to specimen data for research. Over the past two decades, LACMIP has used several different databases to enter and manage specimen catalog records, most recently Microsoft Access and currently Axiell EMu. Cataloging in EMu offers several key benefits over Access, including more consistent and efficient data entry.

# Introduction

If you are new to LACMIP's cataloging workflow, review this section before beginning to create new catalog records.

## Introduction to the Catalogue module
If you are new to EMu, please review documentation for the [Catalogue module]({{ site.baseurl }}/documentation/catalogue/) before proceeding.

## Understanding the ID tag

{% include figure image_path="/assets/images/cataloging_idtag2020.jpg" alt="image of ID tag" caption="Figure showing a blank specimen identification tag. Each highlighted area corresponds to a step or field in the cataloging workflow, explained in more depth below." %}

Cataloging begins with identification tags. As IP staff sort through the collection, they identify specimens and record this information for transcription into the database. It is important that you familiarize yourself with the "anatomy" of these tags before proceeding:

 *ID Tag Field* | *Explanation*
   --- | ---
   **LACMIP loc#.lot#** | Reserved for the **catalog number**, which represents a combination of two numbers: a **locality number** and **lot number**. For example, the catalog number "LACMIP 2533.1" translates to the 1st lot cataloged from LACMIP locality 2533. Likewise, the catalog numbers for the 2nd and 3rd lots cataloged from this same locality would be LACMIP 2533.2, LACMIP 2533.3, and so on. _The lot number is the only thing you will write on the tag during cataloging._
   **Alt #** | Reserved for catalog numbers that were previously assigned to the specimen lot by another institution, e.g. "UCLA 53347".
   **Count** | Reserved for the number of individual specimens in the lot to which a given identification applies, e.g. "3", if 3 _Turritella_ snails are identified. (See documentation for [counting]({{ site.baseurl }}/documentation/digitizing/)).
   **Project** | Refers to the relevant project, typically funding-related, e.g. "FIC" or "WIS"; this value may be pre-printed on the tag.
   **TX/ST** | Refers to the collection in which the specimen lot is to be stored, whereby "ST" = the stratigraphic collection and "TX" = the taxonomic collection.
   **New ID** | Reserved for the specimen lot's identification as assigned by current LACMIP staff; the New ID may be the same as the Old name.
   **ID by** | Reserved for the name of the person who wrote out the ID tag; this name is often pre-printed on the label and includes the date of identification.
   **Old name** | If applicable, this space is reserved for old identifications that were previously assigned to the specimen lot; sometimes this ID is the same as the New ID.
   **Old ID by** | If applicable, this space is reserved for the name of the person who made the old identification. If known, it will also include the date.
   
Above **New ID**, blank space is provided to accomodate **Original Nature** (the fossil's mode of preservation or preparation) and **Anatomy** (anatomical elements). This space is only used when the values for these categories deviate from their default values, "body fossil" and "shell(s)". Likewise, **additional comments** about the taxonomic identification may be written on the back of the specimen tag, to be transcribed into _Comments_ for the **New ID**.

## Two possibilities: to catalog or edit?

There are two possible cataloging scenarios, and looking at the ID tag will tell you which. If the specimen needs a catalog number, only a locality number will be present (e.g., "LACMIP 2533."); the lot number will be blank. In this case, proceed with creating a new catalog record, as outlined immediately below. 

Less commonly, if the specimen was previously cataloged and the existing record needs updating, the catalog number will already be filled out with both a locality and lot number (e.g. "LACMIP 2533.1"). Consult the Collections Manager the first time you think you've encountered this scenario. If this is the case, you will follow the instructions for ["Editing a Catalogue Record"]({{ site.baseurl }}/documentation/cataloging/#editing-a-catalogue-record). 

## Understanding taxonomy
If you are new to taxonomy and binomial nomenclature, please watch the following video and review [this article](https://www.digitalatlasofancientlife.org/learn/systematics/taxonomy/) to familiarize yourself with these concepts before proceeding.
{% include video id="409784937" provider="youtube" %}

# Cataloging

## Creating a new catalogue record

Creating a new catalogue record is the most common kind of cataloging you will do when working with the LACMIP collection, which is enormous and will take years and years of concerted effort to completely catalog. There are a few important things to keep in mind when cataloging:
- Work with one specimen lot (box) at a time. 
- Some boxes contain multiple ID tags, i.e. for some specimens you will be creating multiple catalogue records. Always catalog the top ID tag first.
- **Never remove any labels** from their boxes.
- **Do not reorganize the boxes** within their trays during cataloging.

EMu can facilitate very efficient cataloging if you take a few minutes to set up your workflow. Default values and ditto-ing are two tools to help you do just that, and are explained further down in this section.

### Entering the ID tag data

Begin by creating a new catalogue record (*File > New Record*) and following the step-by-step instructions below. Please note that these are general instructions and you should **always feel free to ask questions** when you are unsure! Also, remember that the documentation for the [Catalogue module]({{ site.baseurl }}/documentation/catalogue/) provides more detailed information about specific fields and possible values that you should also review.

**On the *Invert. Paleo.* tab...**

{% include figure image_path="/assets/images/cataloging_example1_2020.jpg" alt="image of example catalogue record with ID tag" caption="Figure mapping fields from the paper ID tag to their EMu counterparts on the *Invert. Paleo.* tab of the Catalogue module. **Before cataloging for the first time, right-click the image above to enlarge it in a separate tab or window.** An IP staff member can also print it out for you." %}

 *Step* | *On the Invert. Paleo. tab...*
   --- | ---
   1 | Type the LACMIP locality number into the *Locality* field in EMu. You only need to enter the numerals and immediately hit "tab". Pause before moving on; EMu will attach the corresponding [site record]({{ site.baseurl }}/documentation/sites/). Check that the information in this field looks correct, e.g. if you are cataloging material from the Chico Formation and the site record data says "Ladd Formation", that would suggest you mis-typed the locality number.
   2 | Write the auto-generated lot number on the paper ID tag. EMu will populate this in the *Lot No.* field.
   
**Immediately notify an IP staff member if EMu does _not_ generate a lot number, or if you believe it was generated incorrectly**. Lot numbers should always increase sequentially.
{: .notice--warning}

 *Step* | *On the Invert. Paleo. tab...*
    --- | ---
   3 | Enter the *Count* from the paper ID tag into the EMu *Lot Count* field. (The record will not save if you leave this field blank.)
   4 | Check that the EMu *Disp.* (disposition) is "in collection."
   5 | Enter any information next to *Alt #* on the ID tag into the *Inst. Code* and *Inst. Number* fields in EMu.
   6 | Check that the *Collection* field matches what's on paper ID tag. The default value is "ST", so you only need to change it if "TX" is circled. TX (taxonomic) specimens should also have a blue "Moved to Taxonomic Coll." tag in addition to the standard white ID tag. Add lot numbers to these tags are you are cataloging.
   
{% include figure image_path="/assets/images/cataloging_txtag.png" alt="image of example TX tag" caption="All specimens destined for the taxonomic collection should be accompanied by a blue TX tag. Add the lot numbers to these tags when you catalog them." %}

 *Step* | *On the Invert. Paleo. tab...*
    --- | ---
   7 | *Project* depends on the specimens you are cataloging, e.g. "WIS". This value may be pre-printed on the ID tag.
   8 | For *Original Nature*, select "body fossil" unless something else is stated on the ID tag.
   9 | For *Anatomy*, select "shell(s)" unless something else is stated on the ID tag.
   

**On the *Identifications (1)* tab...**

{% include figure image_path="/assets/images/cataloging_example2_2020.jpg" alt="image of example catalogue record with ID tag" caption="Figure mapping fields from the paper ID tag to their EMu counterparts on the *Identifications (1)* tab of the Catalogue module. **Before cataloging for the first time, right-click the image above to enlarge it in a separate tab or window.** An IP staff member can also print it out for you." %}

 *Step* | *On the Identifications (1) tab...*
   --- | ---
   10 | Begin with the *New ID*. Type the name into the *Taxon* field in EMu, e.g. "turritella encina", and press tab. If _only one_ name in the database exists with this exact genus and species combination, the corresponding taxonomy record will automatically be attached after you press tab. If _multiple_ names in the database include this combination (e.g. "turritalla chicoensis"), all possible options in the Taxonomy module will appear, presenting you with all possible choices. The first time this happens, or whenever you are unsure of which name to choose, consult the Collections Manager.
   
If the name written on the tag ends in "**sp.**", you are entering a **genus** (e.g. "Turritella sp."). In this case, only type in the genus name followed by the word "genus", "e.g. turritella genus". (EMu will not understand "Turritella sp.").

If the name written on the tag ends in "**indet.**", you are entering a name that ranks above genus, such as **family** or **order**. Family names typically end in "idae", e.g. "Turritellidae" and "Ostreidae". (EMu will not understand "Turritellidae indet.")
{: .notice--warning}
   
   11 | If the *New ID* includes a modifier (cf., aff.) record it in the EMu *Modifer* field and record the appropriate rank in the *Modifier Rank* field (typically, you would select *Modifier Rank*="genus" or "species"). For more details on modifiers, see the documentation for this field on the [Catalogue module page]({{ site.baseurl }}/documentation/catalogue/).
   12 | Record *ID by* from the paper ID tag in *Identified By*. Names should be formatted "firstname lastname," e.g. "Shawn Wiedrick". This field is a lookup list in EMu, so you can just enter the first name for common identifiers and the field will autocomplete, e.g. type in "Shawn", click on the lookup list icon, and "Shawn Wiedrick" will appear.
   13 | Record the date in *Date Identified* by selecting the calendar icon or typing in the date (DD/MM/YYYY). Dates do not need to include a day or month, i.e. they may be just a year.
   14 | If additional notes are written on the back of the ID tag, record them verbatim in *Comments*.
   15 | Select "Yes" for both *Filed As* and *Currently Accepted*.
   
Every specimen ID tag will have a *New ID* to be entered into the database; only some will also have an *Old name* to enter.
{: .notice--warning}
   
   16 | If an *Old name* has been provided, create a new identification by clicking in the second row of the *Identification List* table. You should see new, empty fields above. As with the first (new) identification, type the taxonomic name into the *Taxon* field in EMu and enter any modifier data into *Modifier* and *Modifier Rank*. For *Old name* only, if the taxon doesn't appear, you may enter "Old name" into the *Taxon* field in EMu and then type out the name into the *Comments* field.
   17 | If *Old ID by* is provided, enter the name (formatted "Firstname Lastname"); enter "unknown" if this field on the ID tag is blank.
   18 | If a date is provided for the *Old ID by*, enter thsi into *Date Identified* in EMu.
   19 | Select "No" for both *Filed As* and *Currently Accepted*.

{% include figure image_path="/assets/images/cataloging_taxonomynotfound_2020.jpg" alt="image of Identifications tab" caption="Example of how to proceed if you come across a taxonomic name on an ID tag that you **cannot find in EMu**. Right-click the image above to enlarge it in a separate tab or window." %}

**If you cannot read the handwriting on the ID tag**, or **no name is returned when you hit tab**, ask for assistance. If no one is immediately available to help: 1) if you are trying to enter a *New ID* into EMu, leave the *Taxon* field blank and enter "TAXONOMY NOT FOUND" followed by the *New ID* in EMu's *Comments* field (e.g. "TAXONOMY NOT FOUND Bittscala sp."; 2) if you are trying to enter an *Old name*, type "Old name" in the *Taxon* field and transcribe whatever is written on the ID tag for *Old name* in EMu's *Comments* field (e.g. "Placenticeras pacificum").
{: .notice--warning}

That's it! Save the catalogue record, **make sure you remembered to record the lot number on the paper ID tag**, and move on to the next specimen.

#### Ditto-ing values

Using EMu's [ditto](http://help.emu.axiell.com/latest/en/Topics/Common/The%20Ditto%20utility.htm?Highlight=ditto) function can help you quickly copy over information from one catalog record to the next. For example...
- You have a tray of EPICC specimen lots to catalog and all belong to the same locality. Ditto the *Invert. Paleo.* tab.
- You have five specimen lots identified as "Turritella encina" by the same person on the same date. Ditto the *Identifications (1)* tab.
- You need to record associated specimen information for 10 specimen lots that are all associated with each other. Ditto the *Lot Remarks* field.

<img src="{{ site.baseurl }}/assets/images/cataloging_ditto.png" alt="" width="300"/>{: .align-right}
To use the ditto function, create a new catalogue record and fill out the fields you want to ditto. A good selection of fields to start with is: *Locality*, *Lot Count*, *Project*, *Original Nature*, *Anatomy*, *Identified By*, and *Date Identified*. **Save this record and set it as your ditto record by going to *Edit > Ditto > Use Current Record for Ditto*.** Make sure that *Update on Save* is not checked (as shown in the image to the right); if it is, the last record you save will always be the record that is being ditto-ed. Finish entering this catalogue record and then when you move to the next ID tag, create a new catalogue record and begin by going to *Edit > Ditto > All Fields*. This will automatically fill in the fields you entered values in your ditto record.

The keyboard shortcut for *Edit > Ditto > All Fields* is *Shift + F9*, or *Shift + Fn + F9*. Using this key command will save you a significant amount of time.
{: .notice--warning}

#### Setting default values

**We recommend that new catalogers stick to using ditto (above) at least until they are more comfortable with EMu!**
{: .notice--warning}

Every EMu user has a base set of default values determined by the Museum's database manager to help us enter data efficiently and consistently. You can add to these base values depending on the specimens you are cataloging. LACMIP base defaults are:

Tab | Field | Value
--- | --- | ---
Invert. Paleo | Collection | ST
Invert. Paleo | Disp. | in collection
Identification (1) | Filed As | Yes
Identification (1) | Currently Accepted | Yes
Security | Publish on Internet | checked (yes)

Setting your own defaults is more complicated than using the ditto tool, but it can be helpful for circumstances where you are always entering the same information, e.g. if you are always cataloging EPICC specimens you could set a default *Project* value of "EPICC." To set your own defaults:
1. Select the *New Record* icon or go to *File > New Record* (you won't actually be creating a new record).
1. Enter the information you want to include by default.
1. Navigate to *Edit > Default Values > Set As Defaults...*.
1. Enter a short descriptive name for your new default in the top field, e.g. "EPICC Base Defaults" You can ignore the two boxes (*Fields* and *Defaults*) and click *OK* to save.
Now when you create a new record EMu will autofill the fields you just set as defaults. EMu will also remember your defaults whenever you log back in, so it may be a good idea to switch back to the base defaults at the end of your cataloging session to avoid accidentally carrying over data from your last cataloging session. To do so, navigate to *Edit > Default Values > Change...* and select "Base Defaults." Never select "No Defaults."

For more on this topic, see Axiell's documentation for [setting defaults in EMu](http://help.emu.axiell.com/v5.1/en/Topics/Common/How%20to%20make%20use%20of%20default%20values.htm).

#### Using key commands

The effective use of key commands will make cataloging both easier and faster. See Axiell's [Keyboard Shortcuts & Quick Reference Guide](http://help.emu.axiell.com/latest/en/Resources/Downloads/Quick%20Reference%20Guide/EMu_QuickRef_Guide_IE_20170629.pdf) in addition to the quick tips below. Keep in mind that not all key commands work on a Mac and/or via the VPN remote access.

Must-have key commands for cataloging include:
- **Move to another tab** using *Ctrl + Shift + [the leading letter of the tab label]*, e.g. *Ctrl + Shift + i* in the Catalogue module will take you to the *Identification (1)* tab.
- **Fill in a tab using ditto** with *Shift + Ctrl + F9*, or *Shift + Ctrl + Fn + F9* on a Mac
- **Fill in all tabs using ditto** with *Shift + F9*, or *Shift + Fn + F9* on a Mac
- **Save** with *Ctrl + s*.
- Create a **new record** with *Crtl + n*.

### Editing a catalogue record

The most common reason that catalogue records need to be edited is to update the lot count and/or identification of a specimen that was cataloged circa 2002-2013. These specimens are frequently interspersed with previously uncataloged specimens in a single tray. There are a few important things to keep in mind when editing catalogue records:
- Some boxes contain multiple ID tags, i.e. for some specimens you may be editing multiple catalogue records.
- Never remove any labels from a specimen box.
- Please do not reorganize the boxes within their trays during cataloging.

In order to edit a catalogue record you first need to find it. Search for the catalogue number (e.g. "26376.19") in the *Cat. No.* field of the EMu [Catalogue module]({{ site.baseurl }}/documentation/catalogue/) in [search mode]({{ site.baseurl }}/documentation/modes/). View the record in edit mode and systematically check that the information on the new ID tag is accurate in EMu. Where it is not–e.g. if the *Lot Count* in EMu is "6" but on the new ID tag it is "3"–update EMu. You will **always** need to add an identification to the EMu catalogue record based on the ID tag *New ID*, *ID By*, and *Date* fields. You will also **almost always** need to update *Disposition* to "in collection."

## Flagging records to print

Any time you create or edit a catalogue record, it also needs to be printed and physically placed with the specimen. [Printing labels]({{ site.baseurl }}/documentation/labels/) is usually done by LACMIP staff on a regular basis, but you will need to mark what records require printing. The best way to do this is to finish your cataloging session and then:
1. Do a new search to find all records where *Modified By* is you and *Modification Date* is today (find these fields on the *Admin* tab).
1. View your search results as a [list]({{ site.baseurl }}/documentation/modes/) in order to visually scan through and confirm that these records look like what you did today. **This is the perfect time to check your work!** Do this by changing the view to _View > List Settings > Choose List_ and select the "QC- Catalogue" option. Sort your records by *Inserted Date-Time* and scan through your entries to check them.
1. Add the search results to a [group]({{ site.baseurl }}/documentation/groups/) by navigating to *Tools > Group > All Records in Results...* and creating a new group called "PRINT - [your name] - [date]" or, if you see the option to, adding your records to an existing group called "PRINT - [your name]."
1. If you created a new group, you'll nee to share this group with whomever will be printing labels. Add access to the group by adding "swiedrick" (or whoever will be printing your labels) on the Security tab of the group's properties.
