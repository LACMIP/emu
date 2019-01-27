---
title: Importing Data
navcat: Basics
tags:
---

*[need content]* Notes from Bill: Your coordinates are actually in nested tables and should be formatted (#:#). The first number is the outer table, the second is the inner table. In your case of prepending data (-:1) means prepend the outer table value, and place the coordinate in row one of the inner table. I’m a little surprised EMu didn’t return an error with only one value (-), but maybe it assumes a missing inner table number equals 1. E.g. LatLatitudeDecimal_nesttab(-:1)
{: .notice--danger}
