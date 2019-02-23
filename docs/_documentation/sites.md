---
title: Sites
navcat: Modules
tags: georeferencing quick-start
last_modified_at: 2019-02-20
---
The Sites module is the primary record for information about specimen collecting localities. Please see [Axiell's documentation](http://help.emu.axiell.com/latest/en/Topics/EMu/Sites%20module.htm) for generic information about this module. Continue reading here to understand how LACMIP uses the fields available in the Sites module.

## IP Locality (1) tab

{% include figure image_path="/assets/images/sites_iplocality1.png" alt="sites module in EMu" caption="Screenshot of the *IP Locality (1)* tab of the Sites module." %}

The *IP Locality (1)* tab provides information about the verbatim locality description, as well as
geographic context. Fields on this tab are...

Loc ID
: The unique number assigned to a collecting event, always prefaced by "LACMIP," e.g. "LACMIP 8199". For invertebrate paleontology collections, each collecting event typically receives its own locality number, since the stratigraphic information may vary even when the geographic information is exactly the same.

Loc Summary
: Not in use.

Uncertain
: A field to track missing or incomplete locality information. When the LACMIP locality registry was migrated into EMu, we created a record for every number in the series to avoid having any gaps; the *Uncertain* box has been checked for any EMu Sites record that did not have a corresponding row in the original locality registry spreadsheet. We are currently working though paper sources to update these uncertain records.

Continent, Country, State/Prov.
: Self-explanatory geographic data fields.

County/Dist.
: County or district-level geographic data, with the administrative unit included, e.g. "Los Angeles County" or "Winn Parish."

City/Town
: An administrative boundaries of the smallest unit, e.g. a park or a city. LACMIP uses this field for aggregating data (e.g. to report to the National Park Service on what specimens we have from NPS property) but not for printing on labels.

NearestPlace
: Land features or sub-administrative units, e.g. a peak or a neighborhood. This field is equivalent to "feature" and is printed out on labels. Units should always be **organized from larger to smaller**, e.g. "Santa Cruz Island, Potato Harbor." When *NearestPlace* includes a **street address** or intersection the city should be included, e.g. "Los Angeles, Bagley Ave & Adams St," even if the city is also included in the *City/Town* field. **Islands** should always be included in *NearestPlace*. Other conventions include **abbreviating road features** (e.g. "St," "US Hwy 101," "CA Hwy 33") and using the value "unknown locality" when the verbatim description is too vague to determine an actual feature from.

Alternate Loc ID
: A table of paired values: *Institution Code* and *Institution Number*. This is common for specimens transferred to LACMIP from other institutions, and is also where you can find field numbers assigned by collectors. Ex: *Institution Code* = "CIT" and *Institution Number* = "5046", or *Institution Code* = "field number" and *Institution Number* = "AH180817."

Geographic Citation
: Attach a bibliography record to the site. Maps are included in the LACMIP EMu bibliography, and also commonly referenced in verbatim localities. If you are attaching a map, **make sure to select the correct year**, e.g. "United States Geologic Survey; 1952; Calabasas" vs. "United States Geologic Survey; 1974; Calabasas." You may need to create a new bibliography record if the map you need to attach does not exist. Publications and/or reports are other common geographic citations.

Source
: The original source for the electronic record, typically a paper registry (e.g. "UCLA locality registry"), a publication (e.g. "Squires & Saul, 2003"), a person (e.g. "Edward C. Wilson (personal communication)"), or field notes (e.g. "Robert J. Stanton Jr. Notebook 6.4"). Other standard values for this field are "assigned by collection manager" and "not recorded."

Verbatim Locality
: The locality description as originally recorded by the collector. Most of the LACMIP site records have been through multiple iterations of digital life, and this data is not truly verbatim anymore, but ideally it includes exactly what the collector recorded, as well as any notes made later by other people (and clearly indicated as such by enclosing the comment in brackets). If relevant multimedia has been attached to the record after the fact, such as emails saved in PDF format, add a descriptive comment to the Verbatim Locality text, e.g. [See attached correspondence from John Alderson.].
<img src="{{ site.baseurl }}/assets/images/sites_verbatim-attachment.png" alt="entering new geographic data" width="500"/>{: .align-right}

### Entering new geographic data

The geography fields (*Continent*, *County*, *State/Prov.*, *County/Dist.*, *City/Town*, and *NearestPlace*) are a massive lookup list, which means that the most effective way to use them is by entering the most specific information you have and letting EMu help you fill in the rest. We recommend that whenever you need to enter new geographic data you use the following steps...

<img src="{{ site.baseurl }}/assets/images/sites_newgeography.png" alt="entering new geographic data" width="400"/>{: .align-right}
1. Enter the *County/Dist.* Click outside of the field to make sure EMu auto-fills the higher geography fields based on *County/Dist.* If it does not, either **(1)** you've entered a county that doesn't yet exist in EMu, **(2)** you made a spelling mistake, or **(3)** the county exists in two different states and you need to select which state you mean by clicking on the lookup list icon next to the *State/Prov.* field.
1. Click on the lookup list icon next to *NearestPlace* to see if the feature you need already exist. If it does, select it. If it doesn't, go ahead and enter it yourself.
1. Check to see if there is a *City/Town* associated with your site in the lookup. Keep in mind that *City/Town* isn't part of the geography lookup list because the information in this field frequently does not fit nicely with a hierarchy, e.g. *NearestPlace* may be a canyon and *City/Town* may be a state park that contains part but not all of the canyon.

FYI used in *NearestPlace*, "area" generally denotes that the locality is within the USGS quad map of the same name, e.g. "Sunland area".
{: .notice--warning}

## IP Locality (2) tab

{% include figure image_path="/assets/images/sites_iplocality2.png" alt="sites module in EMu" caption="Screenshot of the *IP Locality (2)* tab of the Sites module." %}

The *IP Locality (2)* tab provides information about the site's geologic age and lithostratigraphy, as well as township and range coordinate data. Both the *Start/End Age* (*Period*, *Epoch*, *Age*) and *Lithostratigraphic* (*Group*, *Formation*, *Member*) fields belong to lookup lists, which means that if you enter the most specific information first, EMu will fill out the higher level fields. For instance, if you have a site dated to the Turonian, you would enter "Turonian" into *Age* and EMu would fill in *Epoch* = "Late Cretaceous" and *Period* = "Cretaceous." Unfortunately, EMu will not automatically fill out the *End Age* fields based on what you enter for *Start Age*, so you'd need to enter data into those the same way.

More information on the fields in this tab...

Uncertain (Start/End Age)
: Use this to indicate if the age of a site is uncertain.

Period
: The geologic period (a.k.a. system) of the strata that the site was collected from.

Epoch
: The geologic epoch (a.k.a. series) of the strata that the site was collected from.

Age
: The geologic age (a.k.a. stage) of the strata that the site was collected from.

Uncertain (Lithostratigraphic)
: Use this to indicate if the lithostratigraphy of a site is uncertain.

Group
: The geologic group that a formation belongs to. Rarely used by LACMIP.

Formation
: The geologic formation that a site was collected from. If you enter the beginning of a formation name and click the lookup symbol to the right of the field, EMu will bring up a list of options. Selecting from this list helps us maintain consistent data. When entering a new formations, spell out "Formation," e.g. "Ladd Formation."

Member
: The member within a formation, if known. As with *Formation*, best practice is to spell out geologic terms like "Member" or "Sandstone", etc.

LMA
: LMA stands for "Land Mammal Age" but LACMIP uses this field to record biostratigraphic zone data.

Strat. Details
: Any extra information you have concerning the stratigraphy of the site.

TRS
: This nested table includes fields for township and range data.

## Lat/Long tab

{% include figure image_path="/assets/images/sites_latlong.png" alt="sites module in EMu" caption="Screenshot of the *Lat/Long* tab of the Sites module. The top of the tab displays details for the highlighted row in the *Latitude/Longitude List* table (bottom). Note that the *Latitude/Longitude Details* table (top, highlighted in red) is a table nested with a nest table." %}

The *Lat/Long* tab provides information about [georeferencing]({{ site.baseurl }}/documentation/georeferencing/) associated with this site. One site may have multiple instances of georeferencing, typically because it was assigned a preliminary set of coordinates and then revisited to assign higher quality coordinates. Each instance is listed in the *Latitude/Longitude List* table, as shown in the figure above.

Fields on this tab are...

Latitude/Longitude Details
: A nested table of coordinates within the nested table of georeferencing instances. The only reason you should use multiple rows in this table is to describe the vertices of a polygon. Typically LACMIP uses the fields *Latitude (Dec.)* and *Longitude (Dec.)* to record coordinates in decimal degrees, which EMu will automatically convert to degree-minute-second (DMS) format as well. These fields are equivalent to [dwc:decimalLatitude](https://dwc.tdwg.org/terms/#dwc:decimalLatitude) and [dwc:decimalLongitude](https://dwc.tdwg.org/terms/#dwc:decimalLongitude), respecively. We also currently use the *Comment* field to record [dwc:georeferenceVerificationStatus](https://dwc.tdwg.org/terms/#georeferenceVerificationStatus) (i.e. "A categorical description of the extent to which the georeference has been verified to represent the best possible spatial description").

Determination Source
: Equivalent to [dwc:georeferenceSources](https://dwc.tdwg.org/terms/#dwc:georeferenceSources): "	A list (concatenated and separated) of maps, gazetteers, or other resources used to georeference the Location, described specifically enough to allow anyone in the future to use the same resources." At LACMIP this is frequently assumed to be Google Earth, the topo map linked to the site record, and any associated maps attached as multimedia.

Determination Method
: Equivalent to [dwc:georeferenceProtocol](https://dwc.tdwg.org/terms/#dwc:georeferenceProtocol): 	"A description or reference to the methods used to determine the spatial footprint, coordinates, and uncertainties." See lookup list for LACMIP controlled vocabulary, e.g. "LACMIP georeferencing 2019" or "GPS reading in field."

Determined By
: Equivalent to [dwc:georeferencedBy](https://dwc.tdwg.org/terms/#dwc:georeferencedBy): "A list (concatenated and separated) of names of people, groups, or organizations who determined the georeference (spatial representation) for the Location." You will need to attach a Parties record to this field.

Determination Date
: Equivalent to [dwc:georeferencedDate](https://dwc.tdwg.org/terms/#dwc:georeferencedDate): "The date on which the Location was georeferenced."

Radius (Numeric)
: Equivalent to [dwc:coordinateUncertaintyInMeters](https://dwc.tdwg.org/terms/#dwc:coordinateUncertaintyInMeters), i.e. an error radius around the geographic point. **LACMIP radii should always be in meters** (see *Units* below).

Units
: Units for the error radius given in *Radius (Numeric)*. LACMIP radii should always be in meters.

Datum
: Equivalent to [dwc:geodeticDatum](https://dwc.tdwg.org/terms/#dwc:geodeticDatum): "The ellipsoid, geodetic datum, or spatial reference system (SRS) upon which the geographic coordinates given in decimalLatitude and decimalLongitude as based." Most LACMIP georeferencing is done in the "WGS84" datum.

Preferred
: Check "Yes" if this georeference instance is the best available. Only one may be marked preferred. This field determines what coordinates are exported from EMu (at least in the reports we currently have set up).

Notes
: Equivalent to [dwc:georeferenceRemarks](https://dwc.tdwg.org/terms/#dwc:georeferenceRemarks): "Notes or comments about the spatial description determination, explaining assumptions made in addition or opposition to the those formalized in the method referred to in georeferenceProtocol."

Derive Centroid, Centroid Latitude (DMS), Dec., Centroid Longitude (DMS), Dec.
: Leave *Derive Centroid* as the default "System" and don't worry about any of these fields.

Radius (Verbatim), Probability, Geometry
: Ignore these fields; they are going away in the next EMu update.

### Seeing coordinates in Google Maps

EMu will link out to Google Maps for any Site record that has been georeferenced. To use this feature, navigate to *Tools > Resources > Search Google Maps*. You may need to set Chrome as your default browser on the VPN. To do this, open Chrome and follow the instructions to make it your default.

## Notes tab

{% include figure image_path="/assets/images/sites_notes.png" alt="sites module in EMu" caption="Screenshot of the *Notes* tab of the Sites module." %}

The *Notes* tab is a holding area for information about the verbatim collector name(s) and collecting date, formatted collector name(s), verbatim accession number, and digitization project (e.g. "EPICC" or "CSC"). **Eventually this data will be migrated into their own fields**. The only information currently on this tab that will stay on this tab is about who created the record for this site in the former Excel version of the LACMIP locality registry.

## Multimedia tab

{% include figure image_path="/assets/images/sites_multimedia.png" alt="sites module in EMu" caption="Screenshot of the *Multimedia* tab of the Sites module. Double-clicking on the image icon (circled in red, above) will open the media in a larger window." %}

The *Multimedia* tab displays any multimedia records that are attached to this site record, usually **maps with localities marked on them by hand** or **scanned copies of correspondence related to the collecting locality**. These are invaluable resources for georeferencing and otherwise understanding where the site actually is.

## Attachments

<img src="{{ site.baseurl }}/assets/images/sites_attachments.png" alt="viewing attached records" width="400"/>{: .align-right}
You may want to know whether we have cataloged any specimens from a given site. To find out, you can either search by the locality number in the [Catalogue module]({{ site.baseurl }}/documentation/catalogue/), or you can go to *View > Attachments > Current Record*. The latter will bring up a dialog window that looks like the one here, showing you the other modules (and number of records within) that have referenced this site record.
