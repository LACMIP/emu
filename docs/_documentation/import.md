---
title: Importing Data
navcat: Basics
tags:
---

*[need content]* Notes from Bill: Your coordinates are actually in nested tables and should be formatted (#:#). The first number is the outer table, the second is the inner table. In your case of prepending data (-:1) means prepend the outer table value, and place the coordinate in row one of the inner table. I’m a little surprised EMu didn’t return an error with only one value (-), but maybe it assumes a missing inner table number equals 1. E.g. LatLatitudeDecimal_nesttab(-:1)
{: .notice--danger}

Both CUSTOM and TYPICAL imports allow files encoded with either ANSI or UTF-8.  ANSI is the default, but you can select UTF-8 if your import file has Unicode characters (i.e. diacritics, symbols, and many other special characters).   EMu stores the data as Unicode (ANSI characters overlap a subset of UTF-8).

Select CUSTOM
Validate Data or Import
TEST your data before importing.  At a minimum use “Validate Data”.  This option does not import any data.  It only checks the data.
Validate Format: checks for incorrect Field Names
Validate Data:  checks for incorrect Field Names and whether the data is valid (dates are going into date fields, and numbers are going into number fields).  

Import Data:
Choose how attachments are processed during the import.
If your import file includes attachments (…Ref fields, such as SitSiteRef_tab(1).irn) you may select how the EMu import tool handles them.

The defaults are:

None found (no records found in the attachment table) EMu import creates a new record
One Found (only one record found in the attachment table) EMu attaches the found record and continues importing
Many found (multiple records found in the attachment table) EMu pauses and asks which of the found records you want to attach)

Each of these three occurrences can be modified with the “Change” buttons.  As an example, if None found you can change the action to respond with an Error message instead of creating a new record.

Finally, there are two check boxes at the bottom of this screen.

Only search records imported in this batch (by default it is unchecked): Checking this box forces the import to only attach records being created during the current import.  This would prevent the import from searching EMu’s existing records to attach.  It would be extremely rare to check this option.

Exclude empty fields from attachment search (by default it is checked):
If checked the import assumes empty fields are “unknown”, not intentionally empty.  Therefore, an import of Genus and Species where Species is empty means EMu will pause and ask which record that begins with that Genus do you want to attach.
If unchecked the import assumes empty fields are intentionally empty.  Therefore an import of Genus and Species where Species is empty means EMu will attach the Genus record only.

Records
You may choose to process only a portion of your import file.  The default (Starting record = 1, Records to process = 0) will process all records in your import file.

Import Restrictions
The default is None. There are no restrictions.
Check Update if you DO NOT want your import to update records.  In other words, all of your import records should be NEW records.
Check Insert if you DO NOT want your import to create new records.  In other words, all of your import records should update existing records in EMu.

Report

What kind of detail do you want in your Error Report?  Where do you want the report to be created?
Self-explanatory.  However, be aware, the Verbose report can become very large.
