---
title: Publishing Data
navcat: Workflows
tags:
last_modified_at: 2019-02-01
---


The [Integrated Publishing Toolkit (IPT)](https://www.gbif.org/ipt) is what we use to manage collection-level metadata. For example, this is the [LACMIP record on the IPT](http://ipt.idigbio.org/resource?r=lacm-ip), and it feeds [this page on iDigBio](https://www.idigbio.org/portal/recordsets/5082e6c8-8f5b-4bf6-a930-e3e6de7bf6fb) plus [this page on GBIF](https://www.gbif.org/dataset/f0a7ca6e-8da6-4629-97bd-0368705a4d6b).
The IPT is also where Bill uploads successive versions of each collection's specimen dataset (exported from EMu). You can always make changes to what is published by changing the file that is uploaded to the IPT, e.g. if a record was published by accident it can be retracted.

## Setting up a data publishing pipeline

### IPT

1. Get an IPT login.
1. Set up metadata about your collection

### EMu

1. Determine what fields from EMu should be published to iDigBio
This is the most difficult part. You'll need to tell Bill what EMu fields should get translated into which Darwin Core standard fields so that he can write a report to generate the dataset you'll publish. The EMu instances of Malacology and IP are not totally the same, but they're similar, so you'll be able to use our crosswalk (attached) as a starting point. I am also happy to come over to Malacology for a couple hours one day and we could work through this together in that amount of time.

1. Publish specimen data
Bill will export your data from EMu and pass it off to you to verify that the content looks as you expect.
Once you've looked over the data export, Bill will upload the file to the IPT, and your specimen data will be available on the iDigBio Portal as well as on GBIF. iDigBio and GBIF harvest data from the IPT on a regular (usually monthly) basis.

### Images

If you have images associated with specimens, those can also get shared via the IPT, but no need to do both images and data in the same initial publication.


### Ongoing

1. Remember to update what's published, based on whatever frequency makes sense for Malacology (probably at least annually).


*[need content]* Notes from Bill: When I am preparing any NHM data for VertNet or iDigBio I download all of the tables separately. I then verify data was not corrupted and all records are accounted for.  After that the following things are verified: accidental truncation (either before or after exporting), duplication of data, garbage characters, letters where numbers should be, non-dates where dates should be, obvious misspellings, multiple spellings for the same thing (ie US, USA, and “United States” were all entered), data entered in the wrong columns, missing data (ie a locality for Burbank, CA without the County or Country), and I check that every line in associated tables has data and that data is not duplicated on multiple lines.  When I find problems I send them to Staff for review.
{: .notice--danger}
