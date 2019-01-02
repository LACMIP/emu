---
title: Sites Module
tags: module
---

“All of the non-coordinate information (determination source, method, etc) is tied to the single coordinate or coordinates in the Latitude/Longitude Details table at the top.  The Latitude/Longitude Details table is either a single coordinate or multiple coordinates representing a polygon outlining a single area. At the bottom is a list of all the different latitude/longitude groups recorded.  The most common reason I've seen is "historical data".  So, let's say you wanted to retain all the Juan Capriano Reyes data, but now Juanita Capriano Reyes revisited the site and calculated more accurate coordinates.  You can click on the * in the Latitude/Longitude List at the bottom and enter all of the new data given to you by Juanita, while still retaining Juan's original data.”

For individual site spot-checking in the Sites module bring up a record, TOOLS -> RESOURCES -> Search Google Maps. You may need to set Chrome as your default browser on the VPN. To do this, open Chrome and follow the instructions to make it your default.

Second, your import will work as is, but your coordinates are actually in nested tables and should be formatted (#:#).  The first number is the outer table, the second is the inner table.  In your case of prepending data (-:1) means prepend the outer table value, and place the coordinate in row one of the inner table.  I’m a little surprised EMu didn’t return an error with only one value (-), but maybe it assumes a missing inner table number equals 1.

LatLatitudeDecimal_nesttab(-:1)
LatLongitudeDecimal_nesttab(-:1)

The rest are fine --  LatDeterminedByRef_tab(-).irn, LatDetDate0(-), LatRadiusNumeric_tab(-), LatRadiusUnit_tab(-), LatDatum_tab(-), LatPreferred_tab(-), LatLatLongDetermination_tab(-), LatDetSource_tab(-)

LOCALITY TABLE GEOGRAPHY NOTES
islands are always features
township is for administrative boundaries of the smallest unit, e.g. a park or a city
nearest place is for land features or sub-administrative units
"unknown locality" and blank locality are different
"area" should be checked for its use (e.g. "Santa Monica Mountains area")
all townships/features are organized into larger-->smaller when there are commas
road features are abbreviated and sometimes so is mountain
highways are e.g. "US Hwy 101" or "CA Hwy 33"
for features that are street addresses, the city has been included
Reports
[needs content]
