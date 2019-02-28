---
title: Modes of Operation
navcat: Basics
tags: quick-start
last_modified_at: 2019-02-01
---
Each module has four possible screen modes–Search, Display, New, and Edit–depending on your task. These modes are briefly described below, and also covered in the documentation for specific modules.

## Search mode

Search mode allows you to find records, and is the default mode that opening any module will present.

{% include figure image_path="/assets/images/modes_search.png" alt="search mode" caption="Search mode of the Catalogue module in EMu. Note that the two icons circled in red, above, allow you to return to search from your results. The icon with a red x will bring you back to a new search, and the icon without an x will return you to the same search criteria." %}

### Basic operators

Use basic boolean operators to customize your search in EMu. To search **AND**, place both terms on the same line. To search **OR**, place both terms on separate lines. To search **NOT**, place `\!` in front of the term. To search for a specific phrase, use quotes e.g. `\"tuna canyon\"`

### Wildcards

The following wildcards are useful to know when searching EMu. Remember to use the `\` escape character.
- `\*` means any character, e.g. `appl\*` will find "apple," "apply," "application," etc.
- `\*` placed alone means anything, a.k.a. not an empty field
- `\?` means substitute one character, e.g `appl\?` Will find "apple" and "apply"
- `\^` placed at beginning means “starts with”, e.g. `\^card` will find "Card Game", but not "Yellow Card."
- `\$` placed at end means “ends with”, e.g. `card\$` will find "Yellow Card,"" but not "Card Game."
- `\!\*` means not anything, a.k.a. an empty field

Combine wildcards to make your search more specific, e.g. `\^apple\$` returns "apple" but not "apple jar" or "red apple."

### Range searches

You can search numeric fields (i.e. integers) and dates using a range, for example `>=35 <=45` in the *Lot No.* field will search for lot numbers 35 through 45. Or `>=8/1/2015 <= 1/31/2019` in the *Collecting Date* will search for specimens collected between 8/1/2015 and 1/31/2019. Similarly, `26\2-4\]` will return all *LACMIP Type Numbers* from 2626-2640.

### Additional resources

For more details, see [Advanced Searching]({{ site.baseurl }}/documentation/search/), as well as the documentation on searching from Axiell:
- information on [basic search](http://help.emu.axiell.com/latest/en/Topics/Common/How%20to%20search.htm)
- additional information on [advanced searching](http://help.emu.axiell.com/latest/en/Topics/Common/Search%20-%20section.htm)
- [cheatsheet](http://help.emu.axiell.com/latest/en/Resources/Downloads/Unicode/EMu_Unicode_Cheatsheet_IE_20170602.pdf) for search terms

## Display mode

The results of a search are presented to you in display mode, which is a group of records shown by default in list format. Records can also be displayed as a contact sheet view, a page view, or a details view; switch between these views using the display mode icons in the top toolbar (see red circle in figure below). To learn more about each of these views, see [Axiell's documentation](http://help.emu.axiell.com/latest/en/Topics/Common/Displaying%20records.htm).

{% include figure image_path="/assets/images/modes_display.png" alt="display mode" caption="Display mode of the Catalogue module in EMu." %}

### Sorting records

By default, records in display mode are sorted by their IRNs. You can change the sort criteria under either  *Tools > Sort Results* (for sorts you want to be able to share or access frequently) or *Tools > Ad-hoc Sort* (for a sort that you only need to use now). If you'd like to set the default sort to something other than IRN, right-click on one of your sort options and select “Sort After Search”. The selected sort option will be designated by bold text, and will automatically run after every search in this module.

### Adjusting display columns

You can change the columns that are visible in each module's display mode under *View > List Settings*.

If a column displays a nested table, you may need to expand the line height in order to see additional information, e.g. *Cited In* in the Taxonomy Module search results. To increase the line height you can either stretch the row height (grab the bottom of the row and pull) or make the row height much larger in List View properties (*View > List Settings > Choose List > Select List > Properties > Height*).

## Edit mode

If you have permission to edit a record, you will be in edit mode when you enter the "details" view of display mode. Editing field-by-field on a single record is intuitive. For detailed information on what to edit, see the documentation for each module.

{% include figure image_path="/assets/images/modes_edit.png" alt="edit mode" caption="Edit mode of the Catalogue module in EMu." %}

### Global replace

Sometimes you need to make edits that affect multiple records and it would be inefficient to do them field-by-field, record-by-record. For this circumstance, EMu has a powerful tool called [Global Replace](http://help.emu.axiell.com/latest/en/Topics/Common/Global%20Replace.htm). You can easily create unintended consequences, so be careful and read the Axiell documentation (linked above) thoroughly. A few tips for using global replace...
- when you use the global replace tool, it will do *all* replace commands listed, so remember to **clear any past replaces** when you enter a new one.
- to use global replace to **fill blank fields with values**, use *Text to find:* = "^$" and be sure to check the regular expression box.
- see [this article](http://help.emu.axiell.com/latest/en/Topics/Common/Wildcards%20in%20a%20Global%20Replace.htm) for information on advanced global replace using **wildcards**.

### Deleting records

Occasionally you may need to delete a record. Deleting records can be very slow due to EMu’s background validation checks, which run through all module attachments to avoid orphaning records. This takes time. To avoid having deletions be an interruption in your workflow, you can add them to a [group]({{ site.baseurl }}/documentation/groups/) and wait until an appropriate time to delete the entire group of records at once (maybe during lunch or at the end of the day). A similar option is to mark records as “Retired” on the security tab instead of deleting them. A “Retired” record will disappear from all searches and reports, and (if desired), can be deleted overnight. LACMIP does not typically use the retire functionality.

## New mode

Create a new record in any module (that you have the permissions for) by clicking on the icon in the left of the top toolbar. For more information about what data to put in which fields, see the documentation for each module. In general, EMu will let you know if you have forgotten to enter data into a required field, or if your data was entered in the wrong format. Axiell has a basic introduction to editing records in EMu [here](http://help.emu.axiell.com/latest/en/Topics/Common/Working%20with%20records.htm).

{% include figure image_path="/assets/images/modes_new.png" alt="new mode" caption="New mode of the Catalogue module in EMu." %}

### Timesaving tips for new records

Sometimes, data is recorded in a [nested table versus a single field](http://help.emu.axiell.com/latest/en/Topics/Common/Tables.htm). For more information on working with data in this format, see Axiell's documentation (linked above). Rows in a nested table can be copy-pasted into another nested table.

{% include figure image_path="/assets/images/modes_rowcopy.png" alt="copying a row in a nested table" caption="You can copy and paste an entire row from the nested table of one record to another." %}

If you are entering similar data in many new records, consider using the [ditto function](http://help.emu.axiell.com/v5.1/en/Topics/Common/How%20to%20use%20the%20Ditto%20utility.htm), which allows you to set a [record template](http://help.emu.axiell.com/latest/en/Topics/Common/Record%20Templates.htm).
