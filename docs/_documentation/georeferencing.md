---
title: Georeferencing
navcat: Workflows
tags: georeferencing
last_modified_at: 2020-04-14
---
As of late 2018, all LACMIP locality records are maintained in EMu, the collection management system of the NHMLA. However, **georeferencing for LACMIP localities is conducted primarily in Google Earth**, with the Google Earth data being [exported and added back to EMu]({{ site.baseurl }}/documentation/googleearth/) on a regular basis.

LACMIP Google Earth files are set up with both (a) all existing LACMIP georeferenced localities, as well as (b) automatically-generated coordinates for any localities that had not already been georeferenced as of October 2018. These automatically-generated coordinates serve as a starting point and do not need to be preserved beyond their purpose of helping georeferencers determine coordinates by hand.

## Set-up

Begin by finding the most recent version of the LACMIP Google Earth file in *Dropbox > Georeferencing > Google Earth Backups*. The file will be named *LACMIP Google Earth [date].kmz*. Double-clicking on this file will open Google Earth Pro and you should see a folder called *LACMIP Google Earth* under *Temporary Places*. Drag this folder up into *My Places*.

<img src="{{ site.baseurl }}/assets/images/georeferencing_myplaces.png" alt="" width="300"/>{: .align-right}
Within the *LACMIP Google Earth* folder are at least two primary subfolders, *LACMIP Georeferencing* and *Rough Georeferencing*, as well as any additional subfolders that georeferencers are using to organize layers. **Ultimately, we want to migrate all of the placemarks out of the *Rough Georeferencing* folder and into the *LACMIP Georeferencing* folder.**

Locality placemarks in the *Rough Georeferencing* folder were generated automatically by either the [Google Maps API](https://developers.google.com/maps/documentation/geocoding/start) or the [GeoLocate API](http://www.geo-locate.org/), and are extremely variable in quality. Each placemark was assigned a different color upon import into Google Earth: LACMIP Georeferencing placemarks are green, Google Maps placemarks are yellow, GeoLocate Feature placemarks are purple, and GeoLocate Precise placemarks are red.

{% include figure image_path="/assets/images/georeferencing_rough.png" alt="Google Earth georeferencing screenshot" caption="When you click on a placemark from any of the datasets, a window will pop up with metadata about the locality, which is color-coded based on the same scheme as the placemark itself. You can search for placemarks by locality number in the Google Earth search bar." %}

Each placemark in the *Rough Georeferencing* folder has several metadata headers pre-filled in its notes field, as shown in the figure above. We will go over these metadata headers more later.

In addition to having Google Earth running, you will also need to open EMu. For each locality, the state, county, and feature are given in the Google Earth placemark metadata, but you should always have the [EMu Sites module]({{ site.baseurl }}/documentation/sites/) open to check for associated images and to reference the entirety of information about a locality.

## Localities listed in Google Earth

LACMIP staff will help you identify what localities need to be georeferenced. For each of these, you will search for the locality number in Google Earth to see how many of the automated datasets it appears in, then evaluate the placemarks in *Rough Georeferencing* and determine which is "best." **The best placemark should have its coordinates adjusted and metadata added, then be moved into the *LACMIP Georeferencing* folder.** Non-best placemarks can be deleted once reviewed, with the ultimate goal being to have zero placemarks in the *Rough Georeferencing* folder.

Once you have reviewed the rough georeferences and decided which to use as your "best," you should verify that the coordinates are exactly where you wish them to be. You may edit the coordinates of a placemark by clicking on it and selecting *Get Info*. With the info dialog box open (as shown in the figure below) you may either drag the placemark to where it needs to be, or edit the typed coordinates in the dialog box itself.

{% include figure image_path="/assets/images/georeferencing_lacmip.png" alt="Google Earth georeferencing screenshot" caption="Screenshot illustrating what Google Earth should look like when you move a placemark from the *Rough Georeferencing* folder into the *LACMIP Georeferencing* folder and open the *Get Info* dialog box to add metadata." %}

After determining that the coordinates are correct, you need to add metadata to the "best" placemark. You should fill out the following metadata in the notes field of the *Get Info* dialog box by replacing the "XXX" with your own data, e.g.:
- *radius (m)*: XXX; → radius (m): 25;
- *notes*: XXX; → notes: determined based on distance NW of Sam’s cabin;
- *georef date (yyyy-mm-dd)*: XXX; → georef date (yyyy-mm-dd): 2018-12-01;
- *georef by*: XXX; → georef by: Erica Krimmel;

You should **always record the radius, georeference date, and georeferenced by** metadata, but you may not always need to fill out anything in notes. If you do not have information to put in notes, you may leave the default as is (i.e. "notes: XXX;"). Feel free to experiment with copy-pasting metadata into the Google Earth *Get Info* notes field from a sticky note on the desktop or other handy place, but make sure to use the same four metadata headings exactly as they are written here. For example, it might make sense to have "radius (m): XXX; notes: XXX; georef date (yyyy-mm-dd): 2018-12-01; georef by: Erica Krimmel;" ready to copy-paste so that you only need to edit the "XXX" for radius.

## Localities that do not show up in Google Earth

Only about 50% of the total LACMIP localities have any kind of placemark in Google Earth. Placemarks not represented in Google Earth are often foreign, and/or did not have locality data that lended itself to automated georeferencing for a variety of reasons. We will deal with these localities as need be, but if you are working on georeferencing a locality in Google Earth and notice (based on data in EMu) a nearby locality that is not in Google Earth, you may copy the Google Earth placemark, rename it with the additional locality number, and add the appropriate metadata.

## Localities that cannot be georeferenced

Not all site records have sufficient information to georeference. For example, a site with only "Southern California" in *Verbatim Locality* and "Ladd" in *Formation* does not have enough detail to be georeferenced. If you come across sites like this, please note them in the way described below so that we know they have been evaluated.

{% include figure image_path="/assets/images/georeferencing_unable.png" alt="screenshot of EMu record for a site that cannot be georeferenced" caption="Screenshot demonstrating how to fill out fields on the *Lat/Long* tab of the EMu Sites module for a locality that cannot be georeferenced." %}

For a site record where the locality description is too vague to georeference, fill out the following fields on the *Lat/Long* tab...
- *Preferred* = "Yes"
- *Verification Status* = "requires verification" (or "verified by curator" if that applies to you)
- *Determination Source* = "N/A"
- *Determination Method* = "locality description inadequate for georeferencing"
- *Determined By* = attach the Parties record for yourself
- *Determination Date* = select today's date

## Suggested Resources

- [EarthPoint Township & Range on Google Earth](http://www.earthpoint.us/Townships.aspx)
- [LACMIP Locality Registry](http://ip.nhm.org/ipdatabase/locality_show)
- [USGS National Geologic Map Database](https://ngmdb.usgs.gov/ngmdb/ngmdb_home.html)
- [USGS TopoView](https://ngmdb.usgs.gov/topoview/viewer/#4/39.98/-100.06)
- [USGS Feature Query Form](https://geonames.usgs.gov/apex/f?p=138:1:0::NO:::)

