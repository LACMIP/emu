---
title: Google Earth
navcat: Workflows
tags: 
---

1. Download a KML version of the “LACMIP Georeferencing” folder
1. Open the KML file in a text editor and trim it by searching for the first instance of the `<Placemark>` element and deleting everything above this tag and below the `<document>` tag.
1. Import this file to OpenRefine (as XML and highlighting the Placemark element) and run the script called *_OpenRefineScript_GoogleEarth-to-EMu.json*
1. Check data for integrity
1. Select only rows that are after the last Google Earth export (look in EMu > Data Migration Archive > Sites > Georeferencing and at the last date in the file name). Download as a csv.
1. Drop the csv into EMu and open it in Excel
1. Copy the values of the SitSiteNumber column and search for them in EMu. Replace the “Preferred” here to be “No”.
1. Import the csv to the Sites Module via the custom import tool
