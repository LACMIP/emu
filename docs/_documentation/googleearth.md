---
title: Migrating (Google Earth)
navcat: Workflows
tags: georeferencing
toc: false
last_modified_at: 2019-03-01
---
LACMIP uses Google Earth as its primary software for georeferencing, but this data also must be recorded with each LACMIP [Site record]({{ site.baseurl }}/documentation/sites/) in EMu. This page outlines how data generated in Google Earth should be migrated into EMu. See the [georeferencing documentation]({{ site.baseurl }}/documentation/georeferencing/) for more details on how geographic coordinates are assigned to a locality using Google Earth and other tools.

First, open Google Earth and download a KML version of the “LACMIP Georeferencing” folder by right-clicking on it.

{% include figure image_path="/assets/images/googleearth_screenshot.png" alt="screenshot of Google Earth" caption="Screenshot illustrating where to find the LACMIP Georeferencing folder in Google Earth." %}

Open the KML file in a text editor and trim it by searching for the first instance of the `<Placemark>` element and deleting everything above this tag and below the `<Document>` tag. Save the file, then import into OpenRefine and run the script called *[_OpenRefineScript_GoogleEarth-to-EMu.json]({{ site.url_scripts }})*.

{% include figure image_path="/assets/images/googleearth_refinexml.png" alt="screenshot of OpenRefine" caption="Screenshot illustrating how to properly import the KML file into OpenRefine by defining it as XML format and selecting the `<Placemark>` element)" %}

Check data for integrity, then select only rows where the date in *LatDetDate0(-)* is after the last Google Earth export (look in *EMu > Data Migration Archive > Sites > Georeferencing* and at the most recently dated file name). Download this subset of new georeferences as a CSV.

If you are using EMu remotely, log into the VPN and import the CSV to the remote desktop by dragging and dropping it. Open the file in Excel from within the VPN and copy the values of the *SitSiteNumber* column. [Search]({{ site.baseurl }}/documentation/search/) for these values in EMu and make any existing “Preferred” georeferences not preferred, as shown in the figure below. This ensures that the new georeference coordinates get preference over any existing coordinates, which often come from less-accurate batch georeferencing.

{% include figure image_path="/assets/images/googleearth_replacepref.png" alt="screenshot of EMu replace tool" caption="Screenshot of the replace tool set up to find all values of 'Yes' in the *Preferred* field and replace them with 'No.'" %}

Finally, import the CSV into the Sites module via the custom import tool (see [importing data]({{ site.baseurl }}/documentation/import/) for further documentation on this tool).
