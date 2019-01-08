---
title: Google Earth
navcat: Workflows
tags: georeferencing
---
LACMIP uses Google Earth as its primary software for georeferencing collecting localities.

## Migrating data from Google Earth into EMu
1. Open Google Earth and download a KML version of the “LACMIP Georeferencing” folder.
1. Open the KML file in a text editor and trim it by searching for the first instance of the `<Placemark>` element and deleting everything above this tag and below the `<document>` tag.
1. Import this file to OpenRefine as XML (highlighting the `<Placemark>` element), and run the script called *[_OpenRefineScript_GoogleEarth-to-EMu.json]({{ site.url_scripts }})*.
1. Check data for integrity.
1. Select only rows that are after the last Google Earth export (look in *EMu > Data Migration Archive > Sites > Georeferencing* and at the last date in the file name). Download as a CSV.
1. Log into Marconi remote desktop and import the CSV by dragging and dropping it. Open the file in Excel from within Marconi.
1. Copy the values of the *SitSiteNumber* column and search for them in EMu. Replace the “Preferred” here with “No”. This ensures that the new georeference coordinates get preference over any existing coordinates, which often come from less-accurate batch georeferencing.
1. Import the CSV into the Sites Module via the custom import tool.
