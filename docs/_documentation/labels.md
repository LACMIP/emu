---
title: Printing Labels
navcat: Workflows
tags: cataloging
toc: false
---
Printing labels from EMu is simple. First you will need to do a search to bring up the Catalogue records that you want to print labels for. Once you have the search results, select *Tools > Reports* from the top menu. EMu will bring up a dialog box for you to select what kind of report you'd like to generate. Highlight the label report that you want (see below for options) and click either *Report all* to include all records in the search results, or *Report* to include only the records you have selected within the search results. You should now see a new window that looks like the screenshot below.

{% include figure image_path="/assets/images/labels_screenshot.png" alt="image of EMu windows related to printing labels" caption="EMu generates labels as a Crystal report, which then must be printed." %}

The Crystal report window that EMu has opened only gives you a preview of the first page of labels. To print or save your labels, click on the *Print* icon at the top left corner (circled in red in the image above). Leave the settings on the first dialog box (*Page Setup*) as they are and click *OK*. In the second dialog box (*Print*), select *Microsoft XSP Document Writer* and then click *Print*. This will allow you to save the label report as an *XPS* file, which can then be printed.

If you are working via the VPN, you will need to download the *XPS* file onto your local machine and print from there. Please note that you **cannot print this type of file from a Mac computer**. LACMIP labels are set up to use the *XPS* format versus something more portable, e.g. *PDF*, because of restrictions with the remote desktop version of Adobe Acrobat.

## Label report templates

LACMIP currently has two different label templates. These have been created by the Museum's database manager in Crystal Reports; please contact him if you need modifications to either the layout of or the data being pulled into these reports.

**IP Labels Regular** is for the majority of the specimen labels you will print. You should make sure that the specimens in your search results belong to either the "ED", "ST", or "TX" collection when using this label report.

**IP Labels TYPE** is for printing type specimen labels, which have a significantly different layout than regular specimen labels. You should make sure that you only have specimens that belong to the "TYPE" collection in your search results when you are using this label report.

{% include figure image_path="/assets/images/labels_designs.jpg" alt="image of two different specimen label templates" caption="Regular LACMIP specimen label (left) versus LACMIP type specimen label (left)" %}
