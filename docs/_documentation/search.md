---
title: Advanced Searching
navcat: Basics
tags:
last_modified_at: 2019-06-18
---
EMu offers a variety of methods to search for records. Please see the [search mode]({{ site.baseurl }}/documentation/modes/) documentation for an overview, or below for assorted advanced topics. Axiell also has several good resources for learning more about searching in EMu:
- information on [basic search](http://help.emu.axiell.com/latest/en/Topics/Common/How%20to%20search.htm)
- additional information on [advanced searching](http://help.emu.axiell.com/latest/en/Topics/Common/Search%20-%20section.htm)
- [cheatsheet](http://help.emu.axiell.com/latest/en/Resources/Downloads/Unicode/EMu_Unicode_Cheatsheet_IE_20170602.pdf) for search terms

## Additional search

EMu allows you to conduct a search within a search by going to *File > Additional Search.* Select *Merge (OR)...* if you want to add records based on additional search criteria. Select *Intersect (AND)...* if you want to narrow down the records in your current results based on additional search criteria. Select *Subtract (NOT)...* if you want to exclude records based on additional search criteria.

You can also use additional search from the results of a retrieved [group]({{ site.baseurl }}/documentation/groups/).

## List of values

You can copy-paste a list of values into EMu using the *Paste (Insert)* command. To access this command, copy a list either from a spreadsheet or text file (each value needs to be on a new line), then right-click in the field where you want to paste.

{% include figure image_path="/assets/images/search_pasteinsert.png" alt="screenshot of paste-insert" caption="Screenshot illustrating 'Paste (Insert)' command in the EMu search. If the command is grayed out, as it is here, try left-clicking in any other field and then **right**-clicking in the field you wish to paste into." %}

On a Mac laptop you’ll need to click with two fingers on your trackpad to right-click.
{: .notice--warning}

## Numeric range

<img src="{{ site.baseurl }}/assets/images/search_fieldtype.png" alt="" width="300"/>{: .align-right}
You can search for a range of numbers if the field is defined as an integer type (check this by using the arrow-with-question-mark to click in the field and display the type, as shown in the screenshot to the right). To search for a numeric range, use the operators `<`, `=<`, `>`, `>=`, and `=`. For example, to find any records where the value in a field is between 2330 and 2350, inclusive, you would type `>=2330 <=2350` into the EMu search field.

Date fields are also formatted so that you can search by ranges, e.g. entering `>=8/1/2015 <= 1/31/2019` in the *Collecting Date* will search for specimens collected between 8/1/2015 and 1/31/2019.

Some fields that frequently have numbers in them are not technically defined as numeric, which means that you cannot use the basic range search as described above. You can use a regular expression to approximate similar results. For example, the field *LACMIP Type No.* is not defined as an integer because occasionally one specimen has two type numbers, e.g. "3504, 3505." If you wanted to search for the same range as above (any records where the value in a field is between 2330 and 2350) on the *LACMIP Type No.* field you could use the regular expression `23\[3-5\]\?`. What this expression is saying is "look for values that have `23` followed by a single digit that is either `3`, `4`, or `5` followed by any single character."

For more on searching with ranges, see Axiell's documentation [here](http://help.emu.axiell.com/latest/en/Topics/Common/Types%20of%20search.htm).

## Spaces

More advanced searching is required to find consecutive spaces. To do so, in the search form, enter any character in the field you would like to search. Then select *File > Show Search...*; an *Edit Search...* text box will appear. Scroll down to find the name of the field you're trying to search, e.g. *IPCatInstNumber*. Replace `contains '[character you entered in the search form]'` with `like '\*`  `\*'`. (Note: The number of spaces you enter between the `'\*`  `\*'` is the number of spaces EMu will search for). Select OK.

{% include figure image_path="/assets/images/double_spaces.png" alt="edit mode" caption="Example search for consecutive spaces in EMu." %}

## Nested tables

The design of EMu involves nested tables, i.e. a table of values that exists within a record, which is itself a row in a table. For instance, the Catalogue record for LACMIP 2533.1285 is represented in the EMu database as a row in the Catalogue module table, and within this row there is another set of rows holding the data in the *Alternative Numbers* fields.

{% include figure image_path="/assets/images/search_nestedtable.png" alt="screenshot of nested table" caption="EMu's Catalogue module stores *Alternative Numbers* in a nested table with fields for *Inst. Code* and *Inst. Number*." %}

**Nested tables can make searching in EMu  difficult.** Consider a situation where you want to be able to bring up all the site records where there are more than one set of georeferencing coordinates. In other words, you want to search by the number of rows within a nested table. This kind of search requires a report, as does any search that requires pairing values within a nested table, e.g. site records where one of the Lat/Long coordinates has both *Determined By*="Dalton, Trevor" and *Preferred*="No".

## Specimen identifications

Searching for specimens by their taxonomic identification will also bring up records that are identified with related names, i.e. synonyms.

## Attachments

It is often useful to search for records where an attachment exists to another type of record, for example, you may want to see **all localities for which we have cataloged specimens**. To get this data, we need to ask EMu to search for all site records that are attached to a catalogue record.

1. Begin in the Sites module and navigate to the *Objects* tab. If you do not see the *Objects* tab, you can make it visible by going to *View > Attachments > Options > Show Search Tabs*.
1. Attach **all** catalogue records to the Sites search, as illustrated in the screenshot below.
1. Click on the binocular icon to run your search in the Sites module. This is a resource-intensive search and will likely take several minutes.

{% include figure image_path="/assets/images/search_attachments.png" alt="screenshot of searching by attachments in EMu." caption="From the *Objects* tab of the Sites module, click on the green plus icon to bring you to the Catalogue module search. Pull up **all** catalogue records by entering nothing and clicking the binocular icon. Select the search results and attach them to the Sites module using the double green plus icon." %}

### Multimedia attachments

If you want to find all records with multimedia records attached, you can just search for `\+` in the *Title* field of the *Multimedia* tab.

## Saving a search

You may want to save commonly-used search criteria as a group. To learn more about groups, see documentation [here]({{ site.baseurl }}/documentation/groups/).
