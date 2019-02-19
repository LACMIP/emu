---
title: Advanced Searching
navcat: Basics
tags:
last_modified_at: 2019-02-01
---
EMu offers a variety of methods to search for records. Please see the [Search Modes]({{ site.baseurl }}/documentation/modes/) documentation for an overview, or below for assorted advanced topics. Axiell also has several good resources for learning more about searching in EMu:
- information on [basic search](http://help.emu.axiell.com/latest/en/Topics/Common/How%20to%20search.htm)
- additional information on [advanced searching](http://help.emu.axiell.com/latest/en/Topics/Common/Search%20-%20section.htm)
- [cheatsheet](http://help.emu.axiell.com/latest/en/Resources/Downloads/Unicode/EMu_Unicode_Cheatsheet_IE_20170602.pdf) for search terms

## Additional searches

EMu allows you to conduct a search within a search by going to *File > Additional Search.* Select *Merge (OR)...* if you want to add records based on additional search criteria. Select *Intersect (AND)...* if you want to narrow down the records in your current results based on additional search criteria. Select *Subtract (NOT)...* if you want to exclude records based on additional search criteria.

You can also use additional search from the results of a retrieved [group]({{ site.baseurl }}/documentation/groups/).

## List of values

You can copy-paste a list of values into EMu using the **"Paste (Insert)"** command. To access this command, copy a list either from a spreadsheet or text file (each value needs to be on a new line), then right-click in the field for which you want to paste.

{% include figure image_path="/assets/images/search_pasteinsert.png" alt="screenshot of paste-insert" caption="Screenshot illustrating 'Paste (Insert)' command in the EMu search. If the command is grayed out, as it is here, try left-clicking in any other field and then **right**-clicking in the field you wish to paste into." %}

On a Mac you’ll need to click with two fingers on your trackpad to right-click.
{: .notice--warning}

## Nested tables

The design of EMu involves nested tables, i.e. a table of values that exists within a record, which is itself a row in a table. For instance, the Catalogue record for LACMIP 24000.1 is represented in the EMu database as a row in the Catalogue Module table, and within this row there is another set of rows holding the data in the *Alternative Numbers* fields.

{% include figure image_path="/assets/images/search_nestedtable.png" alt="screenshot of nested table" caption="EMu's Catalogue module stores *Alternative Numbers* in a nested table with fields for *Inst. Code* and *Inst. Number*." %}

**Nested tables can make searching in EMu  difficult.** Consider a situation where you want to be able to bring up all the site records where there are more than one set of georeferencing coordinates. In other words, you want to search by the number of rows within a nested table. This kind of search requires a report, as does any search that requires pairing values within a nested table, e.g. site records where one of the Lat/Long coordinates has both *Determined By*="Dalton, Trevor" and *Preferred*="No".

## Specimen identifications

Searching for specimens by their taxonomic identification will also bring up records that are identified with related names, i.e. synonyms.

## Records with attachments

It is often useful to search for records where an attachment exists to another type of record, for example, you may want to see **all localities for which we have cataloged specimens**. To get this data, we need to ask EMu to search for all site records that are attached to a catalogue record.

1. Begin in the Sites module and navigate to the *Objects* tab. If you do not see the *Objects* tab, you can make it visible by going to *View > Attachments > Options > Show Search Tabs*.
1. Attach **all** catalogue records to the Sites search, as illustrated in the screenshot below.
1. Click on the binocular icon to run your search in the Sites module. This is a resource-intensive search and will likely take several minutes.

{% include figure image_path="/assets/images/search_attachments.png" alt="screenshot of searching by attachments in EMu." caption="From the *Objects* tab of the Sites module, click on the green plus icon to bring you to the Catalogue module search. Pull up **all** catalogue records by entering nothing and clicking the binocular icon. Select the search results and attach them to the Sites module using the double green plus icon." %}

## Records with multimedia

The easiest way to find all records (e.g. in the Catalogue module) that have multimedia attached is to search for `\+` in the *Title* field of the *Multimedia* tab.

## Saved searches

You may want to save commonly-used search criteria as a Group. To learn more about groups, see documentation [here]({{ site.baseurl }}/documentation/groups/).
