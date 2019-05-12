---
title: Exporting Data
navcat: Basics
tags: taxonomy
last_modified_at: 2019-05-11
---
There are several primary ways to get data out of EMu: copy-paste, user-created reports, and complex reports using [Crystal Reports](https://www.crystalreports.com/).

Please note that for any of the export methods below, there are a couple extra steps if you are accessing EMu via the VPN. To get a file from the remote desktop of the VPN to your local computer, simply drag it into the folder *This PC > G on Guacamole RDP > Download*. A progress bar will show up in the lower right of the remote desktop, allowing you to click on the filename to transfer it to your local computer.
{: .notice--warning}

## Copy-paste

In the [display mode]({{ site.baseurl }}/documentation/modes/) of any module, you can select records, copy them, and paste them into an Excel document (within the VPN, if you are accessing EMu remotely). Adjust the display columns shown to be able to copy-paste different data. This method is very simple and works well for exports where the information you need exists primarily in a single module.

## EMu reports

For simple information that you want to be able to export as a spreadsheet easily and consistently at any time, creating a report within EMu may be your solution. See [Axiell's documentation](http://help.emu.axiell.com/latest/en/Topics/Common/Three%20ways%20to%20create%20a%20simple%20MS%20Excel%20report%20no%20coding%20required.htm#export) for more.

## Crystal reports

You will need to use Crystal Reports to export information that exists across different modules, and/or  needs to be transformed from the way it is represented in EMu (e.g. different date formats, concatenating fields, etc.). The Museum's database manager designs and maintains Crystal Reports for us; contact him to request edits or additional reports.

{% include figure image_path="/assets/images/export_report.png" alt="screenshot of the reports dialog in EMu" caption="Screenshot showing the *Reports* dialog box in EMu, with the list of available reports highlighted in red. Both user-created and Crystal Reports show up here; you can tell the difference based on the *Type* column." %}

To export data that uses Crystal Reports, you'll first need to do a search to find the records you want to export. From your search results:

1. Go to *Tools > Reports*.
<img src="{{ site.baseurl }}/assets/images/export_save.png" alt="" width="400"/>{: .align-right}
1. Select the report you want to use (see below for available reports).
1. Either click *Report* to only report the records you have selected, or *Report All* to include every record in your search results.
1. Your report will appear in a new window that looks like the screenshot to the right. The data still need to be exported in a usable format; to do so, click on the "save" icon (circled in red in the top image here).
<img src="{{ site.baseurl }}/assets/images/export_csv.png" alt="" width="400"/>{: .align-right}
1. In the save dialog box, you'll need to select a *Format*, usually CSV. Leave the *Destination* as "Disk file" and click *OK*.
1. If you are exporting data as a CSV, you'll get another dialog box. Fill it out as shown in the lower image here, click *OK*, and choose a destination to save the file to.

Once you've told Crystal where to save the export file, a new dialog box will open, showing the progress of the export. Keep in mind that exporting data from EMu is not quick. For example, ~10 minutes to compile 1000 records in a basic data report, or ~15 minutes to compile 3000 records in a taxonomic dictionary report.

For reports that are generated as an Excel or CSV file within the VPN, they are frequently not well-formed, or are formatted for an older version of Excel. To avoid issues with opening the file you may need to open the file in Excel and save as within the VPN first, especially if you are using a Mac computer.
{: .notice--danger}

### Available reports

Listed here are commonly used and maintained LACMIP reports. You will see more than what is here when you open the reports dialog in any module, but many of the default reports are irrelevant to LACMIP.

The following shared reports are available in the [Catalogue module]({{ site.baseurl }}/documentation/catalogue/)...

- **IP Basic Record Output**: (spreadsheet) provides basic specimen occurrence data in [Darwin Core](https://dwc.tdwg.org/) format; same as the data we send to iDigBio/GBIF, but with the full locality information included (lat/lon not truncated and verbatim locality included)
- **IP Cat Num Gaps**: (PDF) lists any gaps in catalog number sequences
- **IP Labels Regular**: (PDF) see documentation for [printing labels]({{ site.baseurl }}/documentation/labels/)
- **IP Labels Type**: (PDF) see documentation for [printing labels]({{ site.baseurl }}/documentation/labels/)

The following shared reports are available in the [Sites module](({{ site.baseurl }}/documentation/sites/))...

- **Earth Map IP**: (kml) opens selected LACMIP localities in Google Earth, if they are georeferenced
- **IP Loc ID Gaps**: (PDF) lists any gaps in the LACMIP locality number sequence; there should never be any, which this report can confirm

The following shared reports are available in the [Taxonomy module](({{ site.baseurl }}/documentation/taxonomy/))...

- **IP Taxonomic Dictionary**: (spreadsheet) provides data in LACMIP taxonomic dictionary format, i.e. including information about occurrences, citations, and synonyms
- **Hierarchy Name and Rank**: (PDF) formatted list of scientific names, arranged according to taxonomic hierarchy and including taxonomic rank information
- **Hierarchy Name Only**: (PDF) formatted list of scientific names, arranged according to taxonomic hierarchy
- **List (A4)/ List (Letter)**: (PDF) formatted list of scientific names and their EMu irns
