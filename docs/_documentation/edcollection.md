---
title: ED Collection
navcat: Workflows
tags: cataloging
toc_sticky: true
last_modified_at: 2021-11-16
---

This documentation explains how to catalog specimens that have very little to no provenance data that are destined for use in LACMIP's education and outreach "ED" collections. Before cataloging any specimens according to this workflow, verify with the curator or collections manager that this is an appropriate step to take. Specimens with research potential should not be cataloged into the ED collection or attached to LACMIP loc. 500,000.

# 1. Load defaults
Begin by creating a new record and loading default values. In the new record, navigate to: _Edit > Default Values > Change_ and select "IP ED Collection". Doing so will pre-populate the record so that several critical values are automatically filled out. These values include:

  Tab | Field | Default Value
  --- | --- | ---
   Invert. Paleo. | _Locality_ | LACMIP 500,000
   Invert. Paleo. | _Disposition_ | in collection
   Invert. Paleo. | _Collection_ | ED
   Invert. Paleo. | _Project_ | Outreach
   Invert. Paleo. | _Lot Remarks_ | ED GEOGRAPHY: unknown; ED UNIT: unknown formation; ED COLLECTOR: unknown; ED DATE: unknown; ED OTHER REMARKS: none;
   Security | _Publish on Internet_ | No

{% include figure image_path="/assets/images/edcollection_defaults1.png" alt="Default values for the LACMIP ED collection" caption="Default Invert. Paleo. tab values for LACMIP specimens to be cataloged into the ED collection and attached to LACMIP loc. 500,000." %}

{% include figure image_path="/assets/images/edcollection_defaults2.png" alt="Default values for the LACMIP ED collection" caption="Default Security tab values for LACMIP specimens to be cataloged into the ED collection and attached to LACMIP loc. 500,000." %}

# 2. Catalog specimen

In addition to the default values outlined above, complete the following:

Tab | _Field_ | Explanation
  --- | --- | ---
   Invert. Paleo. | _Locality_ | Upon creating a new record with the "IP ED Collection" defaults applied, immediately place the cursor into _Locality_ and hit "tab" to generate a new lot number in _Lot No._
   Invert. Paleo. | _Lot Count_ | Enter the lot count based on our standard [counting criteria](({{ site.baseurl }}/documentation/digitizing/#counting/)).
   Invert. Paleo. | _Accn. Lot_ & _Accn. No._ | If the accession number is known _and_ a record for it exists in the [Accession Lots module](({{ site.baseurl }}/documentation/accessions/)), the accession record should be attached to this field and the number number transcribed into _Accn. No._ If no attachment is available in the Accession Lots module, at minimum, transcribe the accession number into _Accn. No._ Refer to the [table below](({{ site.baseurl }}/documentation/edcollection/#ed-accession-data)) for accession numbers commonly associated with the ED collection.
   Invert. Paleo. | _Lot Remarks_ | If any locality information (even very basic information) is known, replace the "unknown" values with whatever is written on the specimen label(s). *If you're able to fill out more than one of the "unknown" fields, the specimen may not be an appropriate candidate for cataloging under LACMIP loc. 500,000 in the ED collection.* Consult the curator or collections manager.
   Invert. Paleo. | _Original Nature_ | Complete this field based on our standard [procedure](({{ site.baseurl }}/documentation/catalogue/#invert-paleo-tab)).
   Invert. Paleo. | _Anatomy_ | Complete this field based on our standard [procedure](({{ site.baseurl }}/documentation/catalogue/#invert-paleo-tab)).
   Identification (1) | various | Complete this tab based on our standard [procedure](({{ site.baseurl }}/documentation/catalogue/#identification-1-tab)).
   
## ED accession data
Accesssion data must be filled out for catalog records attached to LACMIP loc. 500,000 whenever this information is known. A quick reference for commonly used accession numbers for the ED collection is available below. Please ask the collections manager for assistance with verifying accession data before making any assumptions about a specimen's provenance.

Collection | _Accn. Lot_ value
  --- | ---
  Albi | F.A.3978.2005-3
  Maxwell | F.A.3360.2003-2
  Meals | F.A.3817.2001-1
  
# 3. Print labels
Specimens cataloged using this workflow should be accompanied by labels generated using the "IP Labels Regular - ED Coll (Loc 500,000)" report.

# Decomissioning records
If a specimen is cataloged into the ED collection _and_ attached to LACMIP loc. 500,000, is later found to be associated with a more appropriate Sites record, the specimen should be completely recataloged using standard cataloging [procedure](({{ site.baseurl }}/documentation/cataloging)). To decommission the old record attached to LACMIP loc. 500,000:

  Step | Explanation
  --- | ---
  1 | Clear all information from the Invert. Paleo. and Identification (1) tab.
  2 | Change _Disposition_ to "discarded".
  3 | In the _Alternative Numbers_ table, record the new LACMIP catalog number, a la _Inst. Code._ = "LACMIP" and _Inst. Number_ = "#.#".
  4 | Save.


