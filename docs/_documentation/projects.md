---
title: Projects
navcat: Modules
tags: quick-start
last_modified_at: 2020-05-12
---
The Projects module is used to track and report statistics for collections-related research and outreach requests. Only users in the Invertebrate Paleontology permission group can add/enter data in this module.

New users to the Projects module should view previously created records to review examples. Do this by recalling all records of the most relevant project [_Sub-Type_](https://lacmip.github.io/emu/documentation/projects/#project-1-tab) on the search form and viewing the results using the "IP Requests" list view (_View > List Settings > Choose List >_ "IP Requests").

{% include figure image_path="/assets/images/projects_search.png" alt="Search results in the Projects module." caption="Before creating new records, search for existing records in of the same _Sub-Type_ in the Projects module." %}


## Project 1 tab

{% include figure image_path="/assets/images/projects_project1.png" alt="screenshot of the Project 1 tab in the Projects module" caption="Screenshot of the *Project 1* tab in the Projects module." %}

Sub-Type
: A controlled vocabulary to note what type of request or event is being recorded. Values include:
    - "Exhibit"
    - "Field Trip"
    - "Museum Event"
    - "Presentation"
    - "Public Inquiry"
    - "Request (Catalog Numbers)"
    - "Request (Images)"
    - "Request (Loans)"
    - "Request (Locality Numbers)"
    - "Research Visit"
    - "Tour (Carson)"
    - "Tour (NHM)"
    - "Other"
    
Description
: Begin by describing the event or request using an action, e.g. "Sent surface scans of 15 ammonoids to..." Descriptions should be brief and mention any relevant taxa, geologic context, or collections involved in or affected by the request/event, e.g., "...the Stoyanow Collection". When _Sub-Type_="Request (Locality Numbers)", include LACMIP **locality numbers** in this field.


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
: Select the day that the event occurred or the request was fulfilled.


## Objects tab

{% include figure image_path="/assets/images/projects_objects.png" alt="screenshot of the Objects tab in the Projects module" caption="Screenshot of the *Objects* tab in the Projects module." %}

Objects Associated With Project table
: Any cataloged specimen lots associated with the event or request should be attached to this table. Do so by opening the Catalogue module from within the _Object_ field and searching. Sort your results by catalog number. Select all resulting records in the Catalogue module and drag them into the _Objects Associated With Project_ table. **Note:** After the Projects record is saved, it will be visible on the object's [Project tab](https://lacmip.github.io/emu/documentation/catalogue/#project-tab) in the Catalogue module.

**Only attach objects** to records in the Projects module for specimens **that you, researchers, or visitors came in direct contact with** to fullfill a request.
{: .notice--warning}

{% include figure image_path="/assets/images/projects_objects_drag.png" alt="screenshot of the Objects tab in the Projects module" caption="Screenshot of the *Objects* tab in the Projects module." %}

## Statistics tab

{% include figure image_path="/assets/images/projects_statistics.png" alt="screenshot of the Statistics tab in the Projects module" caption="Screenshot of the *Statistics* tab in the Projects module." %}

To fill out the _Project Statistics_ table, it is **highly recommended** that one [**dittos**](http://help.emu.axiell.com/latest/en/Topics/Common/The%20Ditto%20utility.htm?Highlight=ditto) this information from an existing record of the **same Sub-Type**, e.g. "Tour (Carson)", to ensure consistent data entry.
{: .notice--warning}

Type of Statistic
: A table to document basic statistics regarding the event or request. Please take care to complete this information consistently with other records of the same project sub-type. 
    - DURATION: Enter, to the nearest hour, the amount of time spent fullfilling this request/event in _Value_.
    - ATTENDANCE: For outreach events and facility visits, enter the number of attendees in _Value_. In _Comments_, enter names of the primarily individuals involved, e.g. "Kevin Kelley, Patrick Hsieh, SCPS members" or "Nicole Roberts, BIO125 students".
    - REVENUE ($): If an event or request results in revenue for the department, add this number in the _Value_ column with a _Comment_ indicating where the funds were distributed.
    - FACILITIES: If a visit results in use of specific equipment or facilties, list this in _Comments_.
    - AFFILIATION: Enter the affiliation for whomever made the research or outreach request, including internal affiliations, e.g. "NHMLA (Creative Services)", in _Comments_.
