---
title: Field collecting
navcat: Workflows
tags: georeferencing
last_modified_at: 2020-04-27
---

# Using Collector for ArcGIS to capture field localities
Starting in 2020, LACMIP began capturing field localities by utilizing the museum’s ArcGIS Online subscription. Collector is developed by Esri to streamline the field collecting process. This guide will go over how to use the Collector for ArcGIS app when collecting at new localities.

Collector for ArcGIS is available on iOS, iPadOS and Android. This guide will use examples from the iPhone app. 

An ArcGIS Online account is necessary to use the Collector for ArcGIS app. While an account can be shared, Collector does capture the username of who collects points. This can be very useful when checking records for quality. Contact the ArcGIS Online administrator (Bill Mertz) to discuss creating new ArcGIS Online users. 

## Open and Configure Collector
1. Sign in to your ArcGIS Online account
1. Tap the profile button in the upper right corner of the 'Maps' page.
<img src="{{ site.baseurl }}/assets/images/fieldcollecting_collector1.PNG" alt="" width="100"/>{: .align-right}
1. Tap **'Accuracy'** under LOCATION
1. Set the accuracy threshold to the desired distance. **LACMIP's maximum acceptable accuracy radius for georefenced localities is 50 meters**. The default in Collector is set to 30 feet. The accuracy of a collection is determined by the GPS receiver used. Generally speaking, 30 feet is generous threshold. 
1. Tap **'Provider'** under LOCATION.
1. Above is a list of 'Location Providers', or what GPS recievers you have connected. **Integrated** refers to your devices internal GPS, which is not very accurate. If your connected GPS receiver is not listed, tap **Add**. 

## Adding Offline Areas
Collector for ArcGIS allows for capturing field localities offline. To do so, you have to download the area of the map you'll be collecting in. 

To download a web map to your local device:
1. Tap Overflow "..." next to the map you'd like to download. 
1. Zoom into the area of the map you're going to download. 
1. Tap 'Download Area'

## Collecting points
Here are the steps to properly collect a point:
1. Tap the 'Field localities' map from My Maps.
1. To collect a point, tap the + button in the bottom right. 
1. Fill out all applicable fields in the form. (Required fields with have an *)
1. Tap "Add Point"
1. Tap "Submit" in the upper left.

If you do not tap submit then the point will **not be saved**. If it is greyed out, it is likely because not all required fields were filled out. 

## Copying points
Generally speaking, most fields will remain the same between different localities from the say day of collecting. Therefore, the suggested method to collect localities is to fill out all the fields for the first point. From there you can copy that point and "paste" it at the desired location, changing the required fields.

To copy a point:
1. Select the point to be copied
1. Tap the copy button in the center bottom of the form, or scroll to the bottom of the form and tap "Copy". 
1. Follow steps used to normally collect a point. 

## Useful Collector app features

#### Turning on and off layers
By tapping the layers icon in the top navigation bar, you can turn off/on layers (such as geologic overlays you might have uploaded to the 'Field Localities' map. This can be useful if you need to switch between specific overlays/layers.

#### Changing the basemap
1. Tap Overflow "..." in the top navigation bar.
1. Tap "Basemap"
1. Select the desired basemap. 

For our purposes, the "Imagery" basemap can be very useful as it provides aerial imagery. "USA Topo Maps" can also be useful when determining elevation. 

#### Bookmarks
Bookmarks allow users to select areas of a map they'd like to quickly navigate to, rather than having to pan to the location. Bookmarks need to be set in ArcGIS Online or ArcGIS Pro by setting a new map extent and saving it as a bookmark. If they have been set, however, they can be accessed in Collector by:

1. Tap Overflow "..." in the top navigation bar.
1. Tap "Bookmarks"
1. Select the desired bookmark. 

#### Measuring distances
Collector has a tool to measure distances of lines or polygons drawn by the user. This can be very helpful in determining a **rough estimate** of distances. 

1. Tap Overflow "..." in the top navigation bar. 
1. Select "Measure"
1. Tap either the line or polygon button in the lefthand corner.
1. Tap the points of your line/polygon. 
1. Units can be changed by tapping the units (set to mi/sq mi by default) in the lower right.

# Downloading points from ArcGIS Online

