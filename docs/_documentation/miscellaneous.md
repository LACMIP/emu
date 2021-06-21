---
title: Miscellaneous
navcat: Workflows
tags:
toc_sticky: true
last_modified_at: 2021-05-25
---

This page is for EMu documentation the does not yet have a home!

🚧 The documentation on this page is under construction.
{: .notice--warning}


# Catalogue module
## How to "delete" a catalog record & deal with double cataloged lots
Deleting catalog records should be avoided, and especially when a record has already made its way into one of LACMIP's online datasets. However, this occasionally happens, and if you find a lot that falls in this category (i.e. when the accidental catalog number should not be recycled), the "bad" catalog record should be "discarded" in EMu. To do so, made the following changes to the offending catalog record:

| Tab | Field | Change... |
|---|---|---|
| Invert. Paleo. | Disposition | "discarded" |
| Invert. Paleo. | Lot Remarks | Begin your remarks with, "Disregard this catalog record." If needed, add more detail, including the correct catalog number, after this statement. |
| Relationships | Related Records | detach any attached records |
| Security | Publish on Internet | "no" |

Additionally, clear out any values in the following fields on the Invert. Paleo. tab: _LACMIP Type No._, _Field No._, _Alternative Numbers_ table, _Collection_, _Project_, _Original Nature_, _Anatomy_, _IP Publications_ table

🛑 Volunteers and interns do not have permission to delete catalog records, or "discard" them, as outlined above.
{: .notice--warning}

## How to document newly figured and unfigured specimens

As per LACMIP's [citation policy](https://lacmip.github.io/emu/documentation/citing/) citation policy, beginning in 2020, specimens that are published _but not name-bearing types_ (previously known as "hypotypes") will not receive new type numbers and will not be assimilated into the type collection. However, their use in the literature must be documented. Examples of catalog records created for new figured and unfigured specimens to be included in a forthcoming work are below.

Fields to note:

| Tab | Field | Change... |
|---|---|---|
| Invert. Paleo. | LACMIP Type No. | "blank" |
| Invert. Paleo. | Type Status | "figured" or "unfigured" |
| Invert. Paleo. | Collection | "ST" or "TX" (likely "TX" for figured specimens) |
| Invert. Paleo. | Lot Remarks | Specify any updates the record will need after the publication is made available, such as page numbers in the _IP Publications_ table, _Author String_ on new Taxonomy records, or _Title_ on the corresponding Bibliography record. These remarks should be deleted after the changes are made. |

While "figured" and "unfigured" are not official ICZN type statuses, this information must be entered into _Type Status_ for internal insurance valuation purposes.
{: .notice--warning}

{% include figure image_path="/assets/images/imls_newtypefigured.png" alt="" caption="" %}
{% include figure image_path="/assets/images/imls_newtypeunfigured.png" alt="" caption="" %}


# Taxonomy module
## How to create new taxonomy records for the IMLS Project (2019-2021)
{% include figure image_path="/assets/images/imls_newtaxonomy1.png" alt="" caption="" %}
{% include figure image_path="/assets/images/imls_newtaxonomy2.png" alt="" caption="" %}
{% include figure image_path="/assets/images/imls_newtaxonomy3.png" alt="" caption="" %}
{% include figure image_path="/assets/images/imls_newtaxonomy4.png" alt="" caption="" %}
