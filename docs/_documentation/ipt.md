---
title: Publishing Data
navcat: Workflows
tags:
last_modified_at: 2019-02-28
---
The LACMIP collection is a invaluable scientific resource, and strategic collection management helps to make it as accessible as possible. Digitizing specimen data is one way that we can increase accessibility. Published digital data can be used both as-is, and as a finding aid for researchers who may want to visit the collections in person. [iDigBio](http://idigbio.org/) and [GBIF](https://gbif.org) are the two primary portals we where share our collection-level and specimen-level data.

The [Integrated Publishing Toolkit (IPT)](https://www.gbif.org/ipt) is what we use to manage collection-level metadata. For example, this is the [LACMIP resource on the IPT](http://ipt.idigbio.org/resource?r=lacm-ip), which feeds [this page on iDigBio](https://www.idigbio.org/portal/recordsets/5082e6c8-8f5b-4bf6-a930-e3e6de7bf6fb) plus [this page on GBIF](https://www.gbif.org/dataset/f0a7ca6e-8da6-4629-97bd-0368705a4d6b). This metadata lives in the IPT and can be edited there. The IPT also facilitates publishing specimen-level datasets via a CSV file and associated field mapping.

## Setting up a data publishing pipeline

The following is provided for general reference. If you are going through this process you may want to reach out to LACMIP staff and the Museum's database manager for assistance.
{: .notice--warning}

### On the IPT

The IPT is a software for publishing both specimen data and collection-level metadata, as exemplified above. It can be installed on any server; NHMLA is currently using [iDigBio's installation of the IPT](http://ipt.idigbio.org/).

{% include figure image_path="/assets/images/ipt_overview.jpg" alt="diagram showing what the IPT is used for" caption="Diagram illustrating an overview of what we use the IPT for. Please see numerbed text below for a step-by-step explanation." %}

1. Request user accounts on the iDigBio IPT for the NHMLA staff who need access, generally collections managers and informatics staff.
2. Request an IPT "resource" for each collection. When requesting a resource you will need to provide your collection code, which combined with our institution code (LACM) forms a unique shortname, e.g. for Invertebrate Paleontology our collection code is "IP" and our shortname on the IPT is "lacm-ip."
3. Collections staff edit metadata fields directly on the IPT. Refer to the [LACMIP resource on the IPT](http://ipt.idigbio.org/resource?r=lacm-ip) as an example.
4. Informatics staff sets up Darwin Core field mapping (see section below) and uploads a CSV file for each collection dataset that is ready to publish.
5. Biodiversity data aggregators harvest the CSV files and make the data available via their online portals.

### Data in EMu

In addition to setting up your collection resource on the IPT, you also need to determine what fields from EMu should be published. This is the most difficult part of publishing specimen data, but should only need to be done once (and modified when necessary). You will need to work closely with the Museum's database manager to decide what EMu fields should get translated into which [Darwin Core standard](http://rs.tdwg.org/dwc/terms/) fields. For an example, see the [file].

The crosswalk you develop will be coded into an EMu report, which can be run whenever you want to update your published specimen data. It is essential that when you are working on publishing your first dataset you check the report output carefully to catch data quality issues, either with the way the report is set up or with your data itself.

You may not want every record in your EMu Catalogue module to be published. LACMIP excludes records by checking *Publish on Internet* = "No" on the *Security* tab of the Catalogue module. As part of your data verification process, make sure to check that any records which **should not** be published are indeed excluded. Common reasons to exclude records are: specimen has been deaccessioned, specimen is an unsorted bulk sample, specimens are related to in-progress research that requires an embargo, etc.
{: .notice--warning}

Once the data being reported look accurate, the Museum's database manager will upload specimen occurrence file to the IPT, where iDigBio and GBIF harvest data from on a regular basis. Please note that it may be weeks to a month between when your data are uploaded to the IPT and when they become available on the aggregators. Uploading a new specimen occurrence file to the IPT will refresh your published data.

### Including images

If you have images associated with specimens, these can (and should) also get shared via the IPT. Media  metadata is shared in an Audubon Core file, which is uploaded to the IPT separately from your Darwin Core specimen occurrence data. Work with the Museum's database manager to map fields from EMu to Audubon Core; for an example, see [file].

The image files themselves need to be hosted outside of EMu. This protocol is currently under development and this document will be updated when it has been refined.

## Maintaining a data publishing pipeline

Remember to update the data and associated media that you have published based on whatever frequency makes sense for your collection, but probably at least annually. If you are actively digitizing or otherwise making changes/additions to your data in EMu you may want to update your IPT data more frequently.
