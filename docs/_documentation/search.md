---
title: Advanced Searching
navcat: Basic Info
tags:
---
You can search for existing Loc IDs using copy and PASTE (INSERT) in EMu.

Using your Barstow file as an example.
Open the file in Excel
Highlight the SitSiteNumber column and COPY
Open EMu in SEARCH mode
Right-click in Loc ID and select PASTE(INSERT)

Search
Run your Replace

If PASTE(INSERT) is grayed out, left click in any other field then RIGHT-click in Loc ID. If you are on a Mac, you’ll need to click with two fingers on your trackpad to “right click.”

QUESTION: I want to be able to bring up all the catalog records where there is only one identification. How can I do this? My question is specific but also broad, i.e. how can I search for number of rows within a nested table?

ANSWER: Normally it is not possible to run this kind of search (outside of a report).  However, the particular “table” search you want to do is possible due to the nature of the “Filed As” field.

Because “Filed As” is always YES in one ID and always NO if there is any second ID, we can use that to find records with single IDs.

First search for “Filed As” = YES.  This should find all of your records with an ID.  Then FILE-> Additional Search->Subtract(NOT).  Check “Filed As” = NO.

Result is 3,405 records with only “Yes” and no “No” IDs.  Meaning no second IDs.

To verify you can run a single search of “Filed As” = NO.  This will result in all records with a second ID (since “Filed As” must = Yes if there is only one ID).  That result is 695 records, which is the difference of your total 4100 – 3405 = 695.

As noted earlier, other “table” searches aren’t this easy and require a report to determine the table sizes.

Search in Taxonomy for Apis oligocenica
You will find 8 records -- Apis (Synapsis) henshawi henshawi

If you want to search for records actually identified as Apis oligocenica, then place a % in front.
%Apis oligocenica

The % tells EMu not to search for the related names.

The fastest way to find all catalog records that have multimedia attached is to search in catalog TITLE with \+
