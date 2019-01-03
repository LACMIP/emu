---
title: Taxonomy
navcat: Modules
tags:
---

DOCUMENT:
Antiquated distributions (square brackets and note that formation is antiquated), e.g. IRN=203815
REMOVE “antiquated” where it is referring to a formation
Antiquated taxonomy (validity = invalid)
Ditto-ing to add citations from synonym to new valid name
CURRENTLY ACCEPTED
Yes = names that exist (literature or in collection) and that we want printed on a label
No = old names that have a synonym (SOMETIMES two records for one old name will exist when that old name is linked to two current names, see Fulguraria gabbi for an example)
Unknown = only use for names that will never be printed; use sparingly; as a flag to come back to. Cannot attach a valid name.
Use of validity tab
Citation format “STATE: Fm: Subunit” if antiquated use brackets
Rules for carrying forward taxonomic citations
Reports
Taxonomy: Kingdom is in the structure of the data but not visible. Plantae exists and can be found by searching for rank=kingdom

When you update information that affects lower level taxonomy (e.g. changing the order that a family is in) you will need to restart EMu to see the changes take affect.

Search in Taxonomy for Apis oligocenica
You will find 8 records -- Apis (Synapsis) henshawi henshawi

If you want to search for records actually identified as Apis oligocenica, then place a % in front.
%Apis oligocenica

The % tells EMu not to search for the related names.

What does marking a taxonomy record as Currently Accepted?="unknown" do? We were playing around with it on IRN 206195 (which really is a record where we aren't sure what the accepted status should be). In our testing this record became attached on a Pending tab to IRN 202769. What does that mean?

Currently Accepted = “unknown” allows you to have Taxonomic names that have not been verified as synonyms or current names.  They are pending verification.

In the case you described, Tellina ashburnerii was a synonym of Cymbophora ashburneri, but now we do not know what Tellina ashburnerii is a synonym of.  However, Cymbophora ashburneri retains the fact that Tellina ashburnerii was, at one time, a synonym.  I believe  Tellina ashburnerii will disappear from Cymbophora ashburneri’s “pending” list when Tellina ashburnerii is assigned a new current name.

I have not examined “unknown” closely since no other collection manager has found it useful.

Common Names: examples… Blue Jay, Robin, Polar Bear, etc.

Names History: an audit trail of name changes and synonyms.  These fields are filled automatically as taxa become synonyms or are removed from being synonyms.  It’s only helpful if you want to see edit changes.  It doesn’t necessarily reflect actual synonym history since items are placed in this audit trail during edits, even if those edits were entered to fix previous errors.

Primary Citation: Additional fields for information about the Primary Citation.  Original Name, Status, and Type Species (for genera)

Pending: Like Names History, this is automatically filled, and tracks unassigned synonyms.  Unassigned synonyms occur when you make a Currently Accepted name a synonym and you tell EMu NOT to make its heterotypic synonym a synonym of the new Currently Accepted name.  Example: Species C is a heterotypic synonym of Species B.  You then make Species B a synonym of Species A.  EMu will ask you if Species C should also be a synonym of Species A.  If you tell EMu not to, then Species C will be placed in the Pending tab – a synonym “pending” for an accepted name.

There are other tabs that deal with plants and geography.  Although you have plants, I won’t go into them unless you want to.  The Geographic tab appears to be tailored toward living animals (where can the animal be found, and is it endangered)

TO DOCUMENT: citation format, esp. At genus and family level (e.g. species level does not carry up)

The current design of the EMu database cannot support the relationship of one invalid synonym to two valid names. When Bill migrates our Cretaceous synonyms he will create duplicate records for synonyms with this kind of relationship (~50 out of ~1100 synonym names). This is not perfect but seems to be the least bad way to get our data into EMu for now.
Bill testing out what happens to synonyms if the accepted name then becomes a synonym of another name
All old synonyms, as well as the formerly accepted name, become synonyms of the newly accepted name.
