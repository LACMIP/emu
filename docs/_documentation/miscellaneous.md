---
title: Miscellaneous
navcat: Workflows
tags:
toc_sticky: true
last_modified_at: 2021-05-25
---

This page is for EMu documentation the does not yet have a home!

# Catalogue module
## How to "delete" at catalog record & dealing with double cataloged lots
Deleting catalog records should be avoided, especially if that record has already made its way to one of LACMIP's published online datasets. If you find a specimen lot that should be "deleted" (or, more accurately, disregarded) and the accidentaly catalog number should not be recycled, on the "bad" record, make the following changes:

| Tab | Field | Change |
|---|---|---|
| Invert. Paleo. | _Disposition_ | "discarded" |
| Invert. Paleo. | _Lot Remarks_ | Begin the lot remarks with, "Disregard this catalog record." You can add more detail, if needed, including the correct catalog number after this statement. |
| Relationships | _Related Records_ | detach any attached records |
| Security | _Publish on Internet_ | "no" |

Clear out any values in the following fields on the Invert. Paleo. tab: _LACMIP Type No._, _Field No._, _Alternative Numbers_ table, _Collection_, _Project_, _Original Nature_, _Anatomy_, _IP Publications_ table

🛑 **Only staff** should delete or annotate catalog records to be discarded!
{: .notice--warning}
