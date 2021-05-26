---
title: Miscellaneous
navcat: Workflows
tags:
toc_sticky: true
last_modified_at: 2021-05-25
---

This page is for EMu documentation the does not yet have a home!

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

🛑 Volunteers, interns, and part-time stuff should not delete or annotate catalog records to be discarded without assistance.
{: .notice--warning}
