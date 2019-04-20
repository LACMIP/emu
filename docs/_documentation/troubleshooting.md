---
title: Troubleshooting
navcat: Basics
tags: quick-start
last_modified_at: 2019-02-01
---
Listed here are some common issues we have encountered while using EMu. If you are having trouble and none of the issues here apply to you, try searching this documentation website, asking other LACMIP EMu users, or contacting the Museum's database manager, Bill Mertz.

## Problem: VPN time out
You're happily working along in the remote desktop when suddenly the VPN times out, forcing you to sign in again.
{: .notice--warning}

**Solution**: The VPN is set up to log users out automatically after two hours, but it also times out more frequently than that, particularly on computers connected to the internet wirelessly (i.e. the laptops or iMacs at the LACMIP warehouse). The easiest solution is for you to refresh the browser page and log back into the VPN, where you should find EMu still running as you left it.

## Problem: TexAPI error 304/310
You try to log in to EMu but it tells you `TexAPI Error: Cannot get host information (Number 304)` or `Cannot send to remote host (Number 310)`.
{: .notice--warning}

**Solution**: This problem occurs because EMu needs to be shut down properly whenever you exit the remote desktop, otherwise it remains running in the background. Even if the VPN logs you off automatically, you should sign back in to properly exit EMu. If you have been doing so, then this error is likely the result of a network or server issue; in this case, note the time and relay this information to the Museum's database manager or IT.

To solve the issue you'll need to force EMu to quit. Go to *Start > All Programs > Accessories > Command Prompt* in your remote desktop. You will see a black box with a `c: \documents and Settings\` prompt. Type `taskmgr` and press enter. The Windows task manager will appear, with several tabs at the top. The first is *Applications*. If EMu is shown running, click on it to highlight and then select *End Task*. If EMu is not listed here, click on *Processes* to see if it is listed there. Again, if so, highlight it and click *End Process*.

## Problem: TexAPI error -4
You try to log in to EMu but it tells you `TextAPI Error: Can’t open file /home/emu/lacm/loads/fifo/input. Fifo call failed. Expression failed. Validation failed. (Number -4)`.
{: .notice--warning}

**Solution**: EMu is undergoing maintenance and cannot be run. This is a necessary process and should be set up to occur on Saturday nights. Contact the Museum's database manager if you are having problems with this error **not** during Saturday nights, or if you know you will need to access EMu during that timeframe.

## Problem: Can't delete a record
EMu returns an error when you try to delete a record, saying something e.g. `attached to Taxonomy`.
{: .notice--warning}

**Solution**: Because EMu is a relational database, you cannot delete any record that would leave unresolved relationships to other records. In other words, if the bibliography record you are trying to delete is attached to a taxonomy record, EMu will give you an error. To resolve this, figure out where the record you want to delete is attached to and remove these connections.

## Problem: CSV won't import
EMu returns errors when you attempt to  a CSV file.
{: .notice--warning}

**Solution**: If *every* row returns an error, you likely have an issue with the names of your columns. Go back to EMu and check each field name (see [import]({{ site.baseurl }}/documentation/import/) documentation for how to do this) against those in your spreadsheet. Remember that you need to be particularly aware of import columns that reference a module other than the one you are importing into, and that affect fields in nested tables. **If you are unsure how to properly name your columns, contacting the Museum's database manager for help is preferable to accidentally importing a bunch of data into the wrong place.** If only *some* rows return errors, you likely have issues with values in your cells. Try using EMu's import tool "Validate" functionality to see if you can pinpoint the culprit. Check for alpha characters in numeric fields, non-dates in date fields, etc.
