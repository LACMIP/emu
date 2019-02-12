---
title: Importing Catalogue Data
navcat: Basics
tags:
---

*[need content]* Notes from Bill: Your coordinates are actually in nested tables and should be formatted (#:#). The first number is the outer table, the second is the inner table. In your case of prepending data (-:1) means prepend the outer table value, and place the coordinate in row one of the inner table. I’m a little surprised EMu didn’t return an error with only one value (-), but maybe it assumes a missing inner table number equals 1. E.g. LatLatitudeDecimal_nesttab(-:1)
{: .notice--danger}

1. **Prepare to import the data:** Once the CSV file to be imported has been prepared, drag and drop the file into the VPN. It will appear in the "Downloads" folder on the Guacamole server. Move this file to the VPN desktop. Open the CSV file in Excel on the VPN and re-save it. If you're not already working on a wired PC, close the VPN and move to a PC with a **wired internet connection** to complete the import. (If the connection is interrupted, the file may not correctly or completely import.)

2. **In EMu:** *Catalog module > Tools > Import... (find the CSV on the VPN desktop) > Open*. **It is a good idea to import a test file of <5 records (to be deleted before the real import) to ensure your data will import properly.**

3. **Change encoding to UTF-8**

Both CUSTOM and TYPICAL imports allow files encoded with either ANSI or UTF-8.  ANSI is the default, but you can select UTF-8 if your import file has Unicode characters (i.e. diacritics, symbols, and many other special characters).   EMu stores the data as Unicode (ANSI characters overlap a subset of UTF-8).

4. **Import type:** Custom

5. **Validate Data:** Import Data

*Notes from Bill: To Validate Data or Import Data?*
Validate Format: checks for incorrect field names
Validate Data:  checks for incorrect field names and whether the data are valid (dates are going into date fields, and numbers are going into number fields). This option does not import any data; it only checks the data. 
Import Data: Choose how attachments are processed during the import. If your import file includes attachments (…Ref fields, such as SitSiteRef_tab(1).irn) you may select how the EMu import tool handles them.

6. **Attachments:** Use default values (uncheck "Only search records imported in this batch; check "Exclude empty fields from attachment search").

The defaults are:

None found (no records found in the attachment table): EMu import creates a new record
One Found (only one record found in the attachment table): EMu attaches the found record and continues importing
Many found (multiple records found in the attachment table): EMu pauses and asks which of the found records you want to attach)

Each of these three occurrences can be modified with the “Change” buttons.  As an example, if "None found", you can change the action to respond with an Error message instead of creating a new record.

Finally, there are two check boxes at the bottom of this screen.

Only search records imported in this batch (by default it is unchecked): Checking this box forces the import to only attach records being created during the current import.  This would prevent the import from searching EMu’s existing records to attach.  It would be extremely rare to check this option.

Exclude empty fields from attachment search (by default it is checked): If checked the import assumes empty fields are “unknown”, not intentionally empty.  Therefore, an import of Genus and Species where Species is empty means EMu will pause and ask which record that begins with that Genus do you want to attach. If unchecked the import assumes empty fields are intentionally empty.  Therefore an import of Genus and Species where Species is empty means EMu will attach the Genus record only.

7. **Records:** Starting record = 1, Records to process = 0

You may choose to process only a portion of your import file.  The default (Starting record = 1, Records to process = 0) will process all records in your import file.

8. **Import Restrictions:** None

The default is None. There are no restrictions.

Check Update if you DO NOT want your import to update records.  In other words, all of your import records should be NEW records.

Check Insert if you DO NOT want your import to create new records.  In other words, all of your import records should update existing records in EMu.

9. **Report:** Detailed. (The verbose report can become very large.)

10. **Import identifier:** Use the same name as the spreadsheet file (this will make back-tracking easier if something goes awry with this upload), e.g. "FIC-Statz-catalog_2019-02-12"

11. Start

12. Once import is complete, cycle through your records (all or a selection) to make sure the data were correctly imported. The Database Specialist can help you mass delete records if you need to start over. Save all error logs if the import was not successful and you need assistance to undo the import.
