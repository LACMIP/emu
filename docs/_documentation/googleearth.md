---
title: Google Earth to EMu
tags:
---

Download a KML version of the “LACMIP Georeferencing” folder
Open the KML file in a text editor and trim it by searching for the first instance of the <Placemark> tag and deleting everything above this tag and below the <document> tag.
Import this file to OpenRefine (as XML and highlighting the Placemark element) and run the script called _OpenRefineScript_GoogleEarth-to-EMu.json
Check data for integrity
Select only rows that are after the last Google Earth export (look in EMu > Data Migration Archive > Sites > Georeferencing and at the last date in the file name). Download as a csv.
Drop the csv into EMu and open it in Excel
Copy the values of the SitSiteNumber column and search for them in EMu. Replace the “Preferred” here to be “No”.
Import the csv via the custom import tool
