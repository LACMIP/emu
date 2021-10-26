---
title: Sites
navcat: Modules
tags: georeferencing quick-start
last_modified_at: 2020-12-22
---
The Sites module is our primary resource for information about specimen collecting localities. Please see [Axiell's documentation](http://help.emu.axiell.com/latest/en/Topics/EMu/Sites%20module.htm) for generic information about this module. The equivalent [Darwin Core terms](https://dwc.tdwg.org/terms/) are provided where applicable. Continue reading to understand how LACMIP uses the fields available in the Sites module.

## IP Locality (1) tab

{% include figure image_path="/assets/images/sites_IPLocality_2019upgrade.png" alt="sites module in EMu" caption="Screenshot of the *IP Locality (1)* tab of the Sites module." %}

The *IP Locality (1)* tab provides information about the verbatim locality description, as well as
geographic context. Fields on this tab are...

Loc ID
: = [dwc:locationID](https://dwc.tdwg.org/terms/#dwc:locationID)
: The unique number assigned to a collecting event, always prefaced by "LACMIP," e.g. "LACMIP 8199". For invertebrate paleontology collections, each collecting event typically receives its own locality number, since the stratigraphic information may vary even when the geographic information is exactly the same.

Uncertain
: A field to track missing or incomplete locality information. When the LACMIP locality registry was migrated into EMu, we created a record for every number in the series to avoid having any gaps; the *Uncertain* box has been checked for any EMu Sites record that did not have a corresponding row in the original locality registry spreadsheet. We are currently working though paper sources to update these uncertain records.

Continent, Country, State/Prov.
: = [dwc:continent](https://dwc.tdwg.org/terms/#dwc:continent), [dwc:country](https://dwc.tdwg.org/terms/#dwc:country), [dwc:stateProvince](https://dwc.tdwg.org/terms/#dwc:stateProvince)
: Self-explanatory geographic data fields.

County/Dist.
: = [dwc:county](https://dwc.tdwg.org/terms/#dwc:county)
: County or district-level geographic data, with the administrative unit included. Example values include:
- "Ardennes Department"
- "Capital District"
- "Los Angeles County"
- "Southeast Fairbanks Census Area"
- "Staffordshire"
- "Winn Parish"

City/Town
: = [dwc:municipality](https://dwc.tdwg.org/terms/#dwc:municipality)
: An administrative boundary of the smallest unit, e.g. a park or a city. LACMIP uses this field for aggregating data (e.g. to report to the National Park Service on what specimens we have from NPS property). This field may be blank if a locality does not occur within an offical administrative boundary that falls within this category. Example values include:
- "Los Angeles"
- "BLM Public Land, Inyo Mountains Wilderness"
- "Bryce Canyon National Park"
- "Los Padres National Forest, Sespe Wilderness"
- "Makah Indian Reservation"
- "Santa Monica Mountains National Recreation Area, Topanga State Park"
- "Vandenberg Air Force Base"

NearestPlace
: = [dwc:locality](https://dwc.tdwg.org/terms/#dwc:locality)
: Land features or sub-administrative units, e.g. a peak or a neighborhood. This field is equivalent to "feature" and is printed out on labels. Units should always be **organized from larger to smaller**, e.g. "Santa Cruz Island, Potato Harbor" and "Calico Mountains, Mule Canyon". When *NearestPlace* includes a **street address** or intersection the city should be included, e.g. "Los Angeles, Bagley Ave & Adams St," even if the city is also included in the *City/Town* field. **Islands** should always be included in *NearestPlace*. Other conventions include **abbreviating road features** (e.g. "St," "US Hwy 101," "CA Hwy 33") and including **"area"** to denote a locality is within the USGS quad map of the same name (e.g. "Ono area"). If the verbatim locality description is too vague to determine *City/Town* and *NearestPlace*, use the value **"unknown locality"** for *NearestPlace*.

Alternate Loc ID
: = [dwc:locationRemarks](https://dwc.tdwg.org/terms/#dwc:locationRemarks) with the prefix, "Alternate Location ID", e.g., "Alternate Location ID: field number SS-19a-52"
: A table of paired values: *Institution Code* and *Institution Number*. This is common for specimens transferred to LACMIP from other institutions, and is also where you can find field numbers assigned by collectors. Ex: *Institution Code* = "CIT" and *Institution Number* = "1400", or *Institution Code* = "field number" and *Institution Number* = "AH180817".
{% include figure image_path="/assets/images/sites_IPLocality_alternatelocID.png" alt="Examples of old locality numbers recorded in *Alternate Loc ID*" caption="Example of old locality numbers recorded in *Alternate Loc ID* for LACMIP 10446." %}
{% include figure image_path="/assets/images/sites_alternatelocidexample.jpg" alt="Examples of old locality numbers recorded in *Alternate Loc ID*" caption="Examples of old locality numbers recorded in *Alternate Loc ID*. In historic LACMIP collections, these numbers are typically recorded on colored dot labels (green = UCLA; gold = CIT; red = CSUN or another instituion). Note that white, painted-on numbers do not need to be recorded in this field as they represent LACMIP locality numbers." %}

Collectors
: = [dwc:recordedBy](https://dwc.tdwg.org/terms/#dwc:recordedBy) & [dwc:eventDate](https://dwc.tdwg.org/terms/#dwc:eventDate)
: Each LACMIP locality should represent a unique collecting event in time and space. *Names* in this field are formatted as First initial Lastname (for example: A. Hendy, L. Walker). If the collector is unknown, please enter "unknown" in this field. Each locality should also correspond to a specific date; as such, the *Start Date* and *End Date* should be the same, and can be as specific as a day (e.g. 07/18/1946 - 07/18/1946) or as vague as a year (e.g. 1946-1946). Leave this field blank if you do not know when the collecting event took place. *Verbatim* is occasionally used to record collectors names in full as originally recorded, as well as the verbatim original representation of the date and time of the collecting event, e.g. "COLLECTOR: Alexander Stoyanow; DATE: Summer 53" or "DATE: 17-IV-1985"; the contents of this field are not published online.

Geographic Citation
: Attach a [bibliography record]({{ site.baseurl }}/documentation/bibliography/) to the site. Maps are included in the LACMIP EMu bibliography, and also commonly referenced in verbatim localities. If you are attaching a map, **make sure to select the correct year**, e.g. "United States Geologic Survey; 1952; Calabasas" vs. "United States Geologic Survey; 1974; Calabasas." You may need to create a new bibliography record if the map you need to attach does not exist. Publications and/or reports are other common geographic citations.

Source
: The original source for the electronic record, typically a paper registry (e.g. "UCLA locality registry"), a publication (e.g. "Squires & Saul, 2003"), a person (e.g. "Edward C. Wilson (personal communication)"), or field notes (e.g. "Robert J. Stanton Jr. Notebook 6.4"). Other standard values for this field are "assigned by collection manager" and "not recorded."

Verbatim Locality
: = [dwc:verbatimLocality](https://dwc.tdwg.org/terms/#dwc:verbatimLocality); however, LACMIP does not publish this information online. Instead, [dwc:informationWithheld](https://dwc.tdwg.org/terms/#dwc:informationWithheld) is included and autofilled with "verbatim locality description and coordinates withheld but available to researchers upon request".


: The locality description as originally recorded by the collector. Most of the LACMIP site records have been through multiple iterations of digital life, and this data is not truly verbatim anymore, but ideally it includes exactly what the collector recorded, as well as any notes made later by other people (and clearly indicated as such by enclosing the comment in brackets).

{% include figure image_path="/assets/images/sites_verbatim_attachment.png" alt="How to enter new geographic data into *Verbatim Locality*" caption="Enclose new, after-the-fact information in *Verbatim Locality* with square brackets, with the name of whomever made the comment and the date (YYYY-MM-DD) separated by semicolons; e.g. [Presumed to be Waldron, Indiana; A. Hendy; 2017-11-08]" %}

### Entering new geographic data

The geography fields (*Continent*, *County*, *State/Province*, *County/District*, *City/Town*, and *Nearest Place*) are a massive lookup list, which means that the most effective way to use them is by entering the most specific information you have and letting EMu help you fill in the rest. We recommend that whenever you need to enter new geographic data you use the following steps...

<img src="{{ site.baseurl }}/assets/images/sites_newgeography.png" alt="entering new geographic data" width="400"/>{: .align-right}
1. Enter the *County/Dist.* Click outside of the field to make sure EMu auto-fills the higher geography fields based on *County/Dist.* If it does not, either **(1)** you entered a county that doesn't yet exist in EMu, **(2)** you made a spelling mistake, or **(3)** the county exists in two different states and you need to select which state you mean by clicking on the lookup list icon next to the *State/Province* field.
1. Click on the lookup list icon next to *Nearest Place* to see if the feature you need already exists. If it does, select it. If it doesn't, go ahead and enter it yourself.
1. Check to see if there is a *City/Town* associated with your site in the lookup. Keep in mind that *City/Town* isn't part of the geography lookup list because the information in this field frequently does not fit nicely with a hierarchy, e.g. *Nearest Place* may be a canyon and *City/Town* may be a state park that contains part but not all of the canyon.

FYI when used in *Nearest Place*, "area" generally denotes that the locality is within the USGS quad map of the same name, e.g. "Sunland area".
{: .notice--warning}

## IP Locality (2) tab

{% include figure image_path="/assets/images/sites_IPLocality2_2019upgrade.png" alt="sites module in EMu" caption="Screenshot of the *IP Locality (2)* tab of the Sites module." %}

The *IP Locality (2)* tab provides information about the site's geologic age and lithostratigraphy, as well as township and range coordinate data. Both the *Start/End Age* (*Period*, *Epoch*, *Age*) and *Lithostratigraphic* (*Group*, *Formation*, *Member*) fields belong to lookup lists, which means that if you enter the most specific information first, EMu will fill out the higher level fields. For instance, if you have a site dated to the Turonian, you would enter "Turonian" into *Age* and EMu would fill in *Epoch* = "Late Cretaceous" and *Period* = "Cretaceous." Unfortunately, EMu will not automatically fill out the *End Age* fields based on what you enter for *Start Age*, so you'd need to enter data into those the same way.

More information on the fields in this tab...

Uncertain (Start/End Age)
: Use this to indicate if the age of a site is uncertain.

Period
: = [dwc:earliestPeriodOrLowestSystem](https://dwc.tdwg.org/terms/#dwc:earliestPeriodOrLowestSystem) & [dwc:latestPeriodOrHighestSystem](https://dwc.tdwg.org/terms/#dwc:latestPeriodOrHighestSystem)
: The geologic period (a.k.a. system) of the strata that the site was collected from.

Epoch
: = [dwc:earliestEpochOrLowestSeries](https://dwc.tdwg.org/terms/#dwc:earliestEpochOrLowestSeries) & [dwc:latestEpochOrHighestSeries](https://dwc.tdwg.org/terms/#dwc:latestEpochOrHighestSeries)
: The geologic epoch (a.k.a. series) of the strata that the site was collected from.

Age
: = [dwc:earliestAgeOrLowestStage](https://dwc.tdwg.org/terms/#dwc:earliestAgeOrLowestStage) & [dwc:latestAgeOrHighestStage](https://dwc.tdwg.org/terms/#dwc:latestAgeOrHighestStage)
: The geologic age (a.k.a. stage) of the strata that the site was collected from.

Uncertain (Lithostratigraphic)
: Use this to indicate if the lithostratigraphy of a site is uncertain.

Group
: = [dwc:group](https://dwc.tdwg.org/terms/#dwc:group)
: The geologic group that a formation belongs to. Rarely used by LACMIP.

Formation
: = [dwc:formation](https://dwc.tdwg.org/terms/#dwc:formation)
: The geologic formation that a site was collected from. If you enter the beginning of a formation name and click the lookup symbol to the right of the field, EMu will bring up a list of options. Selecting from this list helps us maintain consistent data. When entering a new formations, spell out "Formation," e.g. "Ladd Formation."

Member
: = [dwc:member](https://dwc.tdwg.org/terms/#dwc:member)
: The member within a formation, if known. As with *Formation*, best practice is to spell out geologic terms like "Member" or "Sandstone," etc.

BioStrat Zone
: Used to record biostratigraphic zone data, e.g. "Domengine."

Strat. Details
: Any extra information you have concerning the stratigraphy of the site, such as "2 meters east of LACMIP 42821". Stratigraphic units ranking lower than member (beds) are also captured in this field, e.g. "BED: Espinal Grit".

TRS
: This nested table includes fields for legacy township and range data.

## Lat/Long(2) tab

{% include figure image_path="/assets/images/sites_LatLong2_2019upgrade.png" alt="sites module in EMu" caption="Screenshot of the *Lat/Long* tab of the Sites module. The top of the tab displays details for the highlighted row in the *Latitude/Longitude List* table (bottom). Note that the *Latitude/Longitude Details* table (top, highlighted in red) is a table nested within a nested table." %}

The *Lat/Long(2)* tab provides information about [georeferencing]({{ site.baseurl }}/documentation/georeferencing/) associated with this site. One site may have multiple instances of georeferencing, typically because it was assigned a preliminary set of coordinates and then revisited to assign higher quality coordinates. Each instance is listed in the *Latitude/Longitude List* table, as shown in the figure above.

Fields on this tab are...

Latitude/Longitude Details
: = [dwc:decimalLatitude](https://dwc.tdwg.org/terms/#dwc:decimalLatitude) & [dwc:decimalLongitude](https://dwc.tdwg.org/terms/#dwc:decimalLongitude), respectively, and concatenated into [dwc:verbatimCoordinates](https://dwc.tdwg.org/terms/#dwc:verbatimCoordinates)
: A nested table of coordinates within the nested table of georeferencing instances. The only reason you should use multiple rows in this table is to describe the vertices of a polygon. Typically LACMIP uses the fields *Latitude (Dec.)* and *Longitude (Dec.)* to record coordinates in decimal degrees, which EMu will automatically convert to degree-minute-second (DMS) format as well. These values are truncated to two decimal places when published online, e.g., "33.66, -117.56".

Radius (Numeric)
: = [dwc:coordinateUncertaintyInMeters](https://dwc.tdwg.org/terms/#dwc:coordinateUncertaintyInMeters) 
: An error radius around the geographic point. **LACMIP radii should always be in meters** (see *Units* below). If a locality cannot be placed within a 2500 m radius of uncertainty, it [cannot be georeferenced](https://lacmip.github.io/emu/documentation/georeferencing/#localities-that-cannot-be-georeferenced). Values used by LACMIP include:

 *Value* | *Explanation*
   --- | ---
   5 | Typically applies to localities with GPS-derived coordinates.
   50 | Applies to localities georeferenced with great certainity, but without precise coordinates available.
   2500 | Applies to localities of greatest uncertainty, short of the locality description being inadequate for georeferencing.
   other | Other values (up to 2500 m) may be determined at the discretion of the georeferencer.

Units
: Units for the error radius given in *Radius (Numeric)*. LACMIP radii should always be in meters.

Datum
: = [dwc:geodeticDatum](https://dwc.tdwg.org/terms/#dwc:geodeticDatum)
: "The ellipsoid, geodetic datum, or spatial reference system (SRS) upon which the geographic coordinates given in decimalLatitude and decimalLongitude as based." Most LACMIP georeferencing is done in the "WGS84" datum.

Preferred
: Check "Yes" if this georeference instance is the best available. Only one may be marked preferred. This field determines what coordinates are exported from EMu.

Verification Status
: = [dwc:georeferenceVerificationStatus](https://dwc.tdwg.org/terms/#georeferenceVerificationStatus)
: "A categorical description of the extent to which the georeference has been verified to represent the best possible spatial description". Values used by LACMIP include:

 *Value* | *Explanation*
   --- | ---
   verified by curator | Indicates a locality has been georeferenced within a relatively small radius of uncertainity, typically ≤50 m. i.e., these localities are relatively trustworthy with respect to their accuracy and precision.
   verified by collector | Indicates a locality has been georeferenced within a relatively small radius of uncertainity according to data directly acquired from the collector (e.g., GPS coordinates), typically ≤50 m. i.e., these localities are relatively trustworthy with respect to their accuracy and precision.
   requires verification | Indicates localities of greater uncertainty, typically with a >50 m radius of uncertainty.

Notes
: = [dwc:georeferenceRemarks](https://dwc.tdwg.org/terms/#dwc:georeferenceRemarks)
: "Notes or comments about the spatial description determination, explaining assumptions made in addition or opposition to the those formalized in the method referred to in georeferenceProtocol."

Determination Source
: = [dwc:georeferenceSources](https://dwc.tdwg.org/terms/#dwc:georeferenceSources)
: "A list (concatenated and separated) of maps, gazetteers, or other resources used to georeference the Location, described specifically enough to allow anyone in the future to use the same resources." At LACMIP this is frequently assumed to be Google Earth, the topo map linked to the site record, and any associated maps attached as multimedia.

Determination Method
: = [dwc:georeferenceProtocol](https://dwc.tdwg.org/terms/#dwc:georeferenceProtocol)
: "A description or reference to the methods used to determine the spatial footprint, coordinates, and uncertainties." See lookup list for LACMIP controlled vocabulary, e.g. "LACMIP georeferencing 2019" or "GPS reading in field."

Determination By
: = [dwc:georeferencedBy](https://dwc.tdwg.org/terms/#dwc:georeferencedBy)
"A list (concatenated and separated) of names of people, groups, or organizations who determined the georeference (spatial representation) for the Location." You will need to attach a [Parties]({{ site.baseurl }}/documentation/parties/) record to this field.

Determination Date
: = [dwc:georeferencedDate](https://dwc.tdwg.org/terms/#dwc:georeferencedDate)
: "The date on which the Location was georeferenced."

Derive Centroid
: Leave *Derive Centroid* as the default "System" and don't worry about any of these fields.


### Seeing coordinates in Google Maps

EMu will link out to Google Maps for any Site record that has been georeferenced. To use this feature, navigate to *Tools > Resources > Search Google Maps*. You may need to set Chrome as your default browser on the VPN. To do this, open Chrome and follow the instructions to make it your default.

{% include figure image_path="/assets/images/sites_googlemaps.png" alt="sites module in EMu" caption="How to view a locality with coordinates in Google maps." %}

## Notes tab

{% include figure image_path="/assets/images/sites_notes.png" alt="sites module in EMu" caption="Screenshot of the *Notes* tab of the Sites module." %}

The *Notes* tab is a holding area for information about the verbatim collector name(s) and collecting date, formatted collector name(s), verbatim accession number, and digitization project (e.g. "EPICC" or "CSC"). **Eventually these data will be migrated into their own fields**. The only information currently on this tab that will stay on this tab is about who created the record for this site in the former Excel version of the LACMIP locality registry.

## Multimedia tab

{% include figure image_path="/assets/images/sites_multimedia.png" alt="sites module in EMu" caption="Screenshot of the *Multimedia* tab of the Sites module. Double-clicking on the image icon (circled in red, above) will open the media in a larger window." %}

The *Multimedia* tab displays any multimedia records that are attached to this site record, usually **maps with localities marked on them by hand** or **scanned copies of correspondence related to the collecting locality**. These are invaluable resources for georeferencing and otherwise understanding where the site actually is.

## Station Data tab

{% include figure image_path="/assets/images/sites_stationdata.png" alt="sites module in EMu" caption="Screenshot of the *Station Data* tab of the Sites module." %}

The *Station Data* tab is where accession and other registrar-related numbers are being temporarily stored until a dedicated field is created elsewhere. **Do not add or modify any information on this tab except adding numbers to the *Accn. No.***

Accn. No.
: Every locality associated with accessioned specimens in the collection should have a number in *Accn. No.*, e.g. "L.2586.68-1" or "A.6440.58-5" (whereby "6440" = donor # and "58-5" = the 5th accession from 1958). This number effectively links the location, and therefore its associated specimens, to documentation regarding the museum's legal possession of the specimens. Therefore, when specimens are catalogued, this number should also be entered into *Accn. No.* and, ideally, *Accn. Lot* on the *Invert. Paleo.* tab in the Catalogue module.

## Attachments

<img src="{{ site.baseurl }}/assets/images/sites_attachments.png" alt="viewing attached records" width="400"/>{: .align-right}
You may want to know whether we have cataloged any specimens from a given site. To find out, you can either search by the locality number in the [Catalogue module]({{ site.baseurl }}/documentation/catalogue/), or you can go to *View > Attachments > Current Record*. The latter will bring up a dialog window that looks like the one here, showing you the other modules (and number of records within) that have referenced this site record.
