---
title: Cataloging
navcat: Workflows
tags: cataloging
last_modified_at: 2019-06-25
---

Cataloging (a.k.a. databasing) is a critical step in digitization, and the creation of accurate digital catalog records facilitates both better collection management and easier access to specimen data for research. LACMIP has used several different databases to enter and manage specimen catalog records over the past couple decades, mostly recently Microsoft Access and currently Axiell EMu. Cataloging in EMu offers several key benefits over doing so in Access, including more consistent and efficient data entry.

**Before following the protocol here, please review documentation for the [Catalogue module]({{ site.baseurl }}/documentation/catalogue/).**
{: .notice--warning}

## Understanding the ID tag

{% include figure image_path="/assets/images/cataloging_idtag.jpg" alt="image of ID tag" caption="Figure showing a specimen identification tag, with numbers corresponding to the documentation below." %}

Information to be digitally cataloged is written on the identification tag in each lot. Familiarize yourself with the anatomy of these tags before proceeding:
1. **Catalog number**, a combination of the specimen's locality number and lot number, e.g. "LACMIP 2533.1" (where the locality number is "LACMIP 2533" and the lot number is "1")
2. **Previous number** assigned to the specimen by another institution, e.g. "UCLA 53347"
3. **New ID** assigned by current LACMIP staff; sometimes the same as the Old ID
4. **Old ID** previously assigned to the specimen; sometimes the same as the New ID
5. **Comments** about the taxonomic identification
6. **Edit** box, which is checked if the specimen needs catalogue record edits (vs. to be cataloged anew)
7. **Count** of how many specimens are present (see documentation for [counting]({{ site.baseurl }}/documentation/digitizing/))
8. **Collection**, either "ST" for specimens physically stored in the stratigraphic collection, or "TX" for specimens physically stored in the taxonomic collection
9. **ID By**, or the name of the person who wrote out this label, often pre-printed
10. **Date** of the identification, often pre-printed on the labels

There are two possible cataloging scenarios, and looking at the ID tag will tell you which. If the specimen has never been given a LACMIP catalog number **the *Edit* box will be unchecked** and you will create a new catalogue record, as detailed in the following section. If the specimen was previously cataloged and the existing record needs updating **the *Edit* box will be checked** and you will follow the instructions in the "Editing a Catalogue Record" section, below.

## Creating a new catalogue record

Creating a new catalogue record is the most common kind of cataloging you will do when working with the LACMIP collection, which is enormous and will take years and years of concerted effort to completely catalog. There are a few important things to keep in mind when cataloging:
- Some boxes contain multiple ID tags, i.e. for some specimens you will be creating multiple catalogue records. Always catalog the top ID tag first.
- Never remove any labels from a specimen box.
- Please do not reorganize the boxes within their trays during cataloging.

EMu can facilitate very efficient cataloging if you take a few minutes to set up your workflow smartly. Default values and ditto-ing are two tools to help you do just that, and are explained further down in this section.

### Entering the ID tag data

Begin by creating a new catalogue record (*File > New Record*) and following the step-by-step instructions below. Please note that these are general instructions and you should **always feel free to ask questions** when you are unsure! Also, remember that the documentation for the [Catalogue module]({{ site.baseurl }}/documentation/catalogue/) provides more detailed information that you should review in addition to this.

**On the *Invert. Paleo.* tab...**

{% include figure image_path="/assets/images/cataloging_example2.png" alt="image of example catalogue record with ID tag" caption="Figure mapping fields from the paper ID tag to their EMu counterparts on the *Invert. Paleo.* tab of the Catalogue module. Yellow highlighting indicates fields that you need to fill out but for which information is not recorded on the ID tag." %}

1. Type the LACMIP locality number into the *Locality* field in EMu. You only need to enter the numerals. When you click outside of the field EMu will look up and attach the [site record]({{ site.baseurl }}/documentation/sites/) for this locality. Check that the information in this field looks correct, e.g. if you are cataloging material from the Chico Formation and the site record data says "Ladd Formation" that may be a sign you mis-typed the locality number.
1. Write the lot number on the paper ID tag. EMu will autogenerate this in the *Lot No.* field. Please note that when EMu autogenerates this number is inconsistent, and may be either immediately or at the time you save the record.
1. Enter the *Count* from the paper ID tag into the EMu *Lot Count* field.
1. Check that the EMu *Disp.* (disposition) is "in collection."
1. If the paper ID tag has anything recorded next to *Prev.* enter it in the *Inst. Code* and *Inst. Number* EMu fields.
1. Check that the EMu *Collection* field matches what the paper ID tag says. The default in EMu is "ST" so you really only need to pay attention to tags where "TX" is circled. TX (taxonomic) specimens should also have a blue "Moved to Taxonomic Coll." paper tag in addition to the standard white paper ID tag.
1. *Project* depends on the specimens you are cataloging, e.g. "EPICC".
1. You will almost always be cataloging specimens with a consistent *Original Nature*, typically "body fossil" for mollusks.
1. You will frequently be cataloging specimens with a consistent *Anatomy*, typically "shell(s)" for mollusks.

**On the *Identifications (1)* tab...**

{% include figure image_path="/assets/images/cataloging_example1.png" alt="image of example catalogue record with ID tag" caption="Figure mapping fields from the paper ID tag to their EMu counterparts on the *Identifications (1)* tab of the Catalogue module. Yellow highlighting indicates fields that you need to check but for which information is not recorded on the ID tag." %}

1. Look at the *Old ID* field on the paper ID tag. If it says "null" then you will only be entering one identification in EMu. If it has a name then you will be entering two identifications (one old, one new).
1. Begin with the *New ID*. Type the taxonomic name into the *Taxon* field in EMu. If you know the taxonomic rank, including it will allow EMu to attach the appropriate [taxonomy record]({{ site.baseurl }}/documentation/taxonomy/) automatically, e.g. "turritella encina species" or "turritellidae family." If you do not include the rank then EMu will bring up a taxonomy search for you to select the record  you wish to attach by clicking on the green plus sign icon.

    Figuring out the taxonomic rank for an "indet." name can be tricky, but looking at the last few letters of the name can help. When rank = "family" the name usually ends with "dae," e.g. "Ostreidae." When rank = "order" the name usually ends with "ida," e.g. "Ostreida."
    {: .notice--warning}

1. If the *New ID* includes a modifier (sp., indet., cf., aff.) record it in the EMu *Modifer* field and record the appropriate rank in the *Modifier Rank* field. For more details on modifiers, see the documentation for this field on the [Catalogue module page]({{ site.baseurl }}/documentation/catalogue/).
1. Record *ID by* from the paper ID tag in *Identified By*. Names should be formatted "firstname lastname," e.g. "Shawn Wiedrick." This field is a lookup list in EMu so you can use a shortcut and just enter the last name for common identifiers, e.g. type in "Shawn" and "Shawn Wiedrick" will auto-complete.
1. Record *Date* in *Date Identified*. Dates do not need to include a day or month, i.e. they may be just a year.
1. Record anything in *Comments* on the paper ID tag in the EMu field *Comments*. Please type comments verbatim.
1. Select "Yes" for both *Filed As* and *Currently Accepted*.
1. Move on to the *Old ID*. Create a new identification by clicking in the second row of the *Identification List* table. You should see new, empty fields above. As with the first identification, type the taxonomic name into the *Taxon* field in EMu and enter any modifier data into *Modifier* and *Modifier Rank*.
1. Enter "unknown" as the value for *Identified By*.
1. Do not enter anything for *Date Identified* or *Comments*.
1. Select "No" for both *Filed As* and *Currently Accepted*.

{% include figure image_path="/assets/images/cataloging_taxonomynotfound.png" alt="image of Identifications tab" caption="If you come across a taxonomic name in either the new or old ID that you **cannot find in EMu**, create an identification for it anyway as shown here. Fill out any fields you can, including *Identified By* and *Date Identified*. Then type the name that you cannot find in the *Comments* field, prefaced with 'TAXONOMY NOT FOUND: '." %}

That's it! Save the catalogue record, **make sure you remembered to record the lot number on the paper ID tag**, and move on to the next specimen.

### Ditto-ing values

Using EMu's [ditto](http://help.emu.axiell.com/latest/en/Topics/Common/The%20Ditto%20utility.htm?Highlight=ditto) function can help you quickly copy over information from one catalog record to the next. For example...
- You have a tray of EPICC specimen lots to catalog and all belong to the same locality. Ditto the *Invert. Paleo.* tab.
- You have five specimen lots identified as "Turritella encina" by the same person on the same date. Ditto the *Identifications (1)* tab.
- You need to record associated specimen information for 10 specimen lots that are all associated with each other. Ditto the *Lot Remarks* field.

<img src="{{ site.baseurl }}/assets/images/cataloging_ditto.png" alt="" width="300"/>{: .align-right}
To use the ditto function, create a new catalogue record and fill out the fields you want to ditto. A good selection of fields to start with is: *Locality*, *Lot Count*, *Project*, *Original Nature*, *Anatomy*, *Identified By*, and *Date Identified*. **Save this record and set it as your ditto record by going to *Edit > Ditto > Use Current Record for Ditto*.** Make sure that *Update on Save* is not checked (as shown in the image to the right); if it is, the last record you save will always be the record that is being ditto-ed. Finish entering this catalogue record and then when you move to the next ID tag, create a new catalogue record and begin by going to *Edit > Ditto > All Fields*. This will automatically fill in the fields you entered values in your ditto record.

The keyboard shortcut for *Edit > Ditto > All Fields* is *Shift + F9*, or *Shift + Fn + F9*. Using this key command will save you a significant amount of time.
{: .notice--warning}

### Setting default values

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

### Using key commands

The effective use of key commands will make cataloging both easier and faster. See Axiell's [Keyboard Shortcuts & Quick Reference Guide](http://help.emu.axiell.com/latest/en/Resources/Downloads/Quick%20Reference%20Guide/EMu_QuickRef_Guide_IE_20170629.pdf) in addition to the quick tips below. Keep in mind that not all key commands work on a Mac and/or via the VPN remote access.

Must-have key commands for cataloging include:
- **Move to another tab** using *Ctrl + Shift + [the leading letter of the tab label]*, e.g. *Ctrl + Shift + i* in the Catalogue module will take you to the *Identification (1)* tab.
- **Fill in a tab using ditto** with *Shift + Ctrl + F9*, or *Shift + Ctrl + Fn + F9* on a Mac
- **Fill in all tabs using ditto** with *Shift + F9*, or *Shift + Fn + F9* on a Mac
- **Save** with *Ctrl + s*.
- Create a **new record** with *Crtl + n*.

## Editing a catalogue record

The most common reason that catalogue records need to be edited is to update the lot count and/or identification of a specimen that was cataloged circa 2002-2013. These specimens are frequently interspersed with previously uncataloged specimens in a single tray. There are a few important things to keep in mind when editing catalogue records:
- Some boxes contain multiple ID tags, i.e. for some specimens you may be editing multiple catalogue records.
- Never remove any labels from a specimen box.
- Please do not reorganize the boxes within their trays during cataloging.

In order to edit a catalogue record you first need to find it. Search for the catalogue number (e.g. "26376.19") in the *Cat. No.* field of the EMu [Catalogue module]({{ site.baseurl }}/documentation/catalogue/) in [search mode]({{ site.baseurl }}/documentation/modes/). View the record in edit mode and systematically check that the information on the new ID tag is accurate in EMu. Where it is not–e.g. if the *Lot Count* in EMu is "6" but on the new ID tag it is "3"–update EMu. You will **always** need to add an identification to the EMu catalogue record based on the ID tag *New ID*, *ID By*, and *Date* fields. You will also **almost always** need to update *Disposition* to "in collection."

## Flagging records to print

Any time you create or edit a catalogue record, it also needs to be printed and physically placed with the specimen. [Printing labels]({{ site.baseurl }}/documentation/labels/) is usually done by LACMIP staff on a regular basis, but you will need to mark what records require printing. The best way to do this is to finish your cataloging session and then:
1. Do a new search to find all records where *Modified By* is you and *Modification Date* is today (find these fields on the *Admin* tab).
1. View your search results as a [list]({{ site.baseurl }}/documentation/modes/) in order to visually scan through and confirm that these records look like what you did today.
1. Add the search results to a [group]({{ site.baseurl }}/documentation/groups/) by navigating to *Tools > Group > All Records in Results...* and creating a new group called "PRINT - [your name] - [date]" or, if you see the option to, adding your records to an existing group called "PRINT - [your name]."
1. If you created a new group, you'll nee to share this group with whomever will be printing labels. Add access to the group by adding "swiedrick" (or whoever will be printing your labels) on the Security tab of the group's properties.
