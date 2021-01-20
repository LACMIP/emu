---
title: Projects
navcat: Modules
tags: quick-start
last_modified_at: 2021-01-19
---
The Projects module is used to track and report statistics for collections-related research and outreach requests. Only users in the Invertebrate Paleontology permission group can add/enter data in this module.

New users to the Projects module should view previously created records to review examples. Do this by recalling all records of the most relevant project [_Sub-Type_](https://lacmip.github.io/emu/documentation/projects/#project-1-tab) on the search form and viewing the results using the "IP Requests" list view (_View > List Settings > Choose List >_ "IP Requests").

{% include figure image_path="/assets/images/projects_search.png" alt="Search results in the Projects module." caption="Before creating new records, search for existing records in of the same _Sub-Type_ in the Projects module. Right-click to enlarge this image by opening it in a new tab or window." %}


## Project 1 tab

{% include figure image_path="/assets/images/projects_project1.png" alt="screenshot of the Project 1 tab in the Projects module" caption="Screenshot of the *Project 1* tab in the Projects module." %}

Sub-Type
: A controlled vocabulary to note what type of request or event is being recorded. Values include:

 *Sub-Type* | *For documenting...*
   --- | ---
   Catalog Number | requests to mint new catalog or type numbers
   Destructive Analysis | requests requring destructive analysis and any results, including multimedia (overrides "loan")
   Exhibit | specimen use in temporary and long-term exhibitions
   Field Trip | field outing conducted for research or outreach
   Images | requests for LACMIP staff to capture specimen imagery
   Loans | external and internal loan requests, excluding exhibits
   Locality Numbers | inquiries related to a specific locality/set of localities, as well as the creation of new localities
   Museum Event | offical museum-organized outreach events, e.g. Dino Fest or Scavenger Safari
   New Accession | accession-related activities (overrides "Catalog Number", "Locality Numbers")
   Presentation | invited external presentations
   Public Inquiry | responses to external inquiries that are educational in nature, e.g. interview with K-12 student for their project
   Record Search | requests for occurrence data and anscillary information, e.g. inventory, taphonomic, or faunal surveys
   Research Visit | in-person research visits to the collections at Carson and NHM
   Tour (Carson) | tours of collections facility in Carson
   Tour (NHM) | tours of IP Type Room at NHM
   Other | unusual collections-based requests and events
   
   
Description
: Begin by describing the event or request using an action, e.g. "Sent surface scans of 15 ammonoids to..." Descriptions should be brief and mention any relevant taxa, geologic context, or collections involved in or affected by the request/event, e.g., "...the Stoyanow Collection". Requests fulfilled for mitigation firms should begin with "MITIGATION:".


## Project 2 tab

{% include figure image_path="/assets/images/projects_project2.png" alt="screenshot of the Project 2 tab in the Projects module" caption="Screenshot of the *Project 2* tab in the Projects module." %}

Organisers
: Attach the appropriate Parties records for whomever fullfilled the request or participated in the event.

Funding Associations
: Attach the appropriate Parties records for any funding sources related to the request or event whenever applicable. **Tip:** If you enter "Cretaceous" in this field and hit tab, the record for the "Connecting the Cretaceous Seas" PEN will appear. That said, always open the full Parties record to check that the correct funding source was attached. New [Parties]({{ site.baseurl }}/documentation/parties/) records can only be added by the database administrator.

Intended Audience
: For outreach-related requests and events, select the appropriate value from the controlled vocabulary:
    - "Advancement/Donors"
    - "Educators"
    - "General public"
    - "Students"
    - "Other" (e.g., use for internal NHMLA tours)
    - "N/A" (use for research-related requests and staff-only field trips)
    

## Dates tab

{% include figure image_path="/assets/images/projects_dates.png" alt="screenshot of the Dates tab in the Projects module" caption="Screenshot of the *Dates* tab in the Projects module." %}

Commencement Date
: Select the day that the collections/research-related request was initiated or the outreach event occurred.

Notification Date (=End Date)
: Do not use this field, except when specifying the end dates for exhibits, loans, and field trips.


## Objects tab

{% include figure image_path="/assets/images/projects_objects.png" alt="screenshot of the Objects tab in the Projects module" caption="Screenshot of the *Objects* tab in the Projects module." %}

Objects Associated With Project nested table
: Any cataloged specimen lots associated with the event or request should be attached to this table. Do so by opening the Catalogue module from within the _Object_ field and searching. Sort your results by catalog number. Select all resulting records in the Catalogue module and drag them into the _Objects Associated With Project_ table. **Note:** After the Projects record is saved, it will be visible on the corresponding [Project tab](https://lacmip.github.io/emu/documentation/catalogue/#project-tab) on the Catalogue records.

**Only attach Catalogue records** for specimens **that were physically handled** to fullfill requests.
{: .notice--warning}

{% include figure image_path="/assets/images/projects_objects_drag.png" alt="screenshot of the Objects tab in the Projects module" caption="Screenshot of the *Objects* tab in the Projects module." %}

## Statistics tab

{% include figure image_path="/assets/images/projects_statistics.png" alt="screenshot of the Statistics tab in the Projects module" caption="Screenshot of the *Statistics* tab in the Projects module." %}

**Highly Recommended:** The easiest way to complete the _Project Statistics_ table is to [**ditto**](http://help.emu.axiell.com/latest/en/Topics/Common/The%20Ditto%20utility.htm?Highlight=ditto) this information from an existing record of the **same Sub-Type** to ensure consistent data entry!
{: .notice--warning}

Type of Statistic table
: A table to document basic statistics regarding an outreach event or research request. Not every type of statistic is required for every Projects record. _Please take care to complete this information consistently with other records of the same project sub-type._ 
    - ATTENDANCE: For outreach events, enter the number of attendees in _Value_. In _Comments_, enter names of the primarily individuals involved, e.g. "Kevin Kelley, Patrick Hsieh, SCPS members" or "Nicole Roberts, BIO125 students". For research requests, only enter the names of the individual(s) who made the request in _Comments_.
    - AFFILIATION: For all events and requests, record the affiliation of whomever made the request in the _Comments_ field, e.g. "USGS, NHMLA (Malacology)".
    - CONTACT: For loans, record contact information in the _Comments_ field.
    - DURATION (hrs): For outreach events, enter, to the nearest hour, the amount of time spent fullfilling this request/event in _Value_.
    - FACILITIES: If a visit results in use of specific equipment or facilties, list this in _Comments_.
    - LOCALITIES: Record locality numbers created for field trips, new accessions, and other specific requests to mint new locality numbers, or locality numbers used for specific record searches.
    - REGISTRAR: Record any relevant registrar numbers here, including accession ("A.#", "F.A.#", etc.) and loan numbers ("L.#").
    - REVENUE ($): If an event or request results in revenue for the department, add the amount in the _Value_ column with a _Comment_ indicating where the account to which the funds were allocated.

## Multimedia tab

{% include figure image_path="/assets/images/projects_multimedia.png" alt="screenshot of the Multimedia tab in the Projects module" caption="Screenshot of the *Multimedia* tab in the Projects module." %}

Attach relevant multimedia to the Multimedia tab, e.g. results of destructive analyses, license agreements, internal movement reciepts, etc. If many files need to be attached, compress them into a ZIP file prior to importing into EMu. Uncompressed versions of the files should also be archived in Extensis Portfolio. When desirable, specimen images should be attached to the appropriate Catalogue records instead of the Projects record.
