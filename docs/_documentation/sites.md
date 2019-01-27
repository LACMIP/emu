---
title: Sites
navcat: Modules
tags: georeferencing quick-start
---
The Sites module is the primary record for information about specimen collecting localities. Please see [Axiell's documentation](http://help.emu.axiell.com/latest/en/Topics/EMu/Sites%20module.htm) for generic information about this module.

*[need content]*
{: .notice--danger}

## Geographic data conventions

The following are conventions followed by LACMIP while cleaning locality data in preparation to migrate into EMu:
- *City/Town* is for **administrative boundaries** of the smallest unit, e.g. a park or a city; it is used for aggregating data but not usually printed on labels
- *NearestPlace* is for **land features** or **sub-administrative units**, e.g. a peak or a neighborhood; it is equivalent to "feature" and what is printed out on labels
- data in *City/Town* and *NearestPlace* are organized from larger to smaller units, e.g. "Santa Cruz Island, Potato Harbor"
- when *NearestPlace* includes a street address or intersection, the city should be included, e.g. "Los Angeles, Bagley Ave & Adams St"
- islands are always included in the *NearestPlace* field
- "unknown locality" and a null locality have different meanings
- when used in *NearestPlace*, "area" generally denotes that the locality is within the USGS quad map of the same name (e.g. "Sunland area"); this has not always been applied as evenly
- road features are typically abbreviated, e.g. "St" instead of "Street"
- highways are formatted e.g. "US Hwy 101" or "CA Hwy 33"

## Google Maps

EMu will link out to Google Maps for any Site record that has been georeferenced. To use this feature, navigate to *Tools > Resources > Search Google Maps*. You may need to set Chrome as your default browser on the VPN. To do this, open Chrome and follow the instructions to make it your default.
