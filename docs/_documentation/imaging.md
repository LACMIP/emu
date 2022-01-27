---
title: Imaging
navcat: Workflows
tags: imaging
toc_sticky: true
last_modified_at: 2021-12-23
---

This page will help get you started with specimen photography.

# Basic photography
This workflow will introduce you to the basic steps required to image fossils using our Nikon D610 DSLR camera combined with the Nikkor AF Micro-Nikkor 60mm f/2.8D lens.

*Step* | *Workflow task...*
   --- | ---
   Hardware | Uncover camera station. Turn on: 1) the camera and uncap lens and 2) the lights attached to the copy stand.
   Software | On the Mac desktop, initiate: 1) *Camera Control Pro 2* with LiveView ("LV") enabled and 2) open the _Pictures_ folder (_Macintosh HD > Users > lacmipvolunteers > Pictures_). You may need to manually move the camera up/down on the copy stand in order to position the template within the window like this.
   Select | LACMIP staff will assign you a set of specimens to image. If the specimens are presented to you in a tray or drawer, please do not rearrange the boxes as you work through them, **only work with one specimen lot at a time, and never disassociate specimens from their labels.** Immediately alert the Collections Manager if you think a specimen and its labels have become mismatched.
   Position | <img src="{{ site.baseurl }}/assets/images/imaging_cameracontrol.png" alt="" width="600"/>{: .align-center} Orient the specimen in the frame of the image using LiveView. _If you are unfamiliar with imaging fossil invertebrates_, refer to the LACMIP [image gallery](https://www.gbif.org/occurrence/gallery?dataset_key=f0a7ca6e-8da6-4629-97bd-0368705a4d6b) on GBIF for examples. The [Digital Atlas of Ancient Life](https://www.digitalatlasofancientlife.org/learn/mollusca/) also has good examples and introductory anatomical explanations.
   Barcode | Place the specimen label in the field of view such that the barcode is completely visible in the corner of the image. The barcode must not be visually obscured in any way. At this point, your desktop should look something like [this]({{ site.baseurl }}/assets/images/imaging_desktop.png).
   Capture | In the LiveView window, click on the barcode. A box will appear over it. Select "AF and Shoot". If the image is not captured, you may need to select a different focal point with the mouse.
   QC| The new image will appear in the _Pictures_ folder. Quickly quality control (QC) the image to ensure both the barcode and specimen are in focus. (If they are not, click on another focal point in the Camera Control Pro window and capture another photo until everything is in focus.) Please immediately delete images that are not in focus. **If the barcode is not in focus, the image will not be renamed properly.**
   Repeat | Repeat the steps above until all necessary views are captured for the specimen. Typically 1-2 views are captured for bivalves (interior & exterior) & 2-3 views for gastropods (apertural & abapterural, plus an umbilical view for Trochoidea & Patellogastropoda). If a lot contains multiple specimens, and overall ("habitus") image showing all specimens may be required. If there is a pink tag in the box, remove it before moving onto the next specimen lot.
   Labels | If you have been instructed to image the accompanying labels, include the "labels" barcode on the image template. If labels have text on two sides, photograph both sides. If there are too many labels to fit into the field of view, please take multiple images until all labels are captures. 
   Save | At the end of your imaging session, all files need to be saved to _Google Drive > LACMIP Imaging_ in the appropriate folder directory. Select all new images in _Pictures_ and drag them into the appropriate "To Process" folder in _LACMIP Imaging_. The files will be automatically renamed and moved overnight. 
   Delete | Once your files have successfully copied to Google Drive (save the last 10 mins of your shift for this task), delete your originals from the _Pictures_ folder before leaving. **Do not delete them until every file has been uploaded.**
   Shut Down | When your imaging shift is complete, replace the lens cap and dust cover on the camera and turn off the lights. Because this is a shared workstation, please keep it tidy!

:warning: **Handle all imaging equipment with care.** The cameras and lenses are difficult to clean and costly to replace. Never remove the lenses from the cameras or touch the glass on either lens.
{: .notice--warning}

:fax: If you need to print new scale bars, label barcodes, etc., or refresh the background template because it's worn, these items are saved in _Google Drive > LACMIP Imaging_.
{: .notice--warning}

# Macrophotography

Photographing small specimens and taking detailed images of larger specimens requires a more involved and time-consuming workflow. These images are acquired using a Canon EOS 5D Mark III DSLR camera paired with a Canon MP-E 65mm f/2.8 1-5x macro lens and a Cognysis StackShot macro rail. A [guide to macrophotography](https://drive.google.com/file/d/1VsrV8OBMxUAjes_QLagHZisrnTrAbwyv/view?usp=sharing) was developed for LACMIP's Fossil Insect PEN (2017-2020).

Additionally, the museum's Keyence microscope can be accessed by appointment when very high quality imagery is needed to fulfill research requests. Access to this equipment is controlled by the [Entomology](https://nhm.org/research-collections/departments/entomology) division.
   
# Storage
## Google Drive
All specimen images should be saved to an appropriate subfolder in _Google Drive > Shared Drives > LACMIP Imaging_. **The purpose of this shared drive is to store original, unaltered specimen images**. These files should be periodically shared with the Database Manager for ingestion into EMu's [Multimedia module]({{ site.baseurl }}/documetation/multimedia). Images that are intended for the web will also need to be uploaded to Extensis Portfolio.

{% include figure image_path="assets/images/imaging_sharing.png" alt="screenshot showing where to save images" caption="**Save images to the appropriate folder in the shared Google Drive, _LACMIP Imaging_** Right-click the image above to enlarge it in a separate tab or window." %}

## Extensis Portfolio
[Extensis Portfolio](https://www.extensis.com/portfolio) is the NHMLA's institutional DAMS. All images to be shared with online aggregators must have [metadata]({{ site.baseurl }}/documetation/imaging/#metadata) applied before ingestion into Extensis.

You can [acccess Extensis](https://digitalgallery.nhm.org:9443/#/) using your NHMLA login and password. Not all images in Extensis are publicly visible; **only files save to the catalog "Inverpaleo published assets" will become available online**, whereas files saved to "Invertpaleo archived assets" will remain private. Files added to the former catalog can be viewed and downloaded from [here](http://digitalgallery.nhm.org:8085/invertpaleo_nhm/#/), and can be pushed to aggregators.

The first time you access Extensis, ask IT (itsupport@nhm.org) for the best contact for direct assistance with the DAMS. This individual can provide advice on the latest recommendations for ingesting large batches of images into Extensis, and should be able to adjust any permissions you need enabled within the DAMS.

## Other copies
Prior to the NHMLA's adoption of Google Drive in 2019, images for the EPICC (2015-2020), CSC (2017-2019), and FIC (2017-2020) projects were saved to two external hard drives. These files have since been backed up on the DAMS and in Google Drive. LACMIP will _not_ be using external hard drives for long-term image storage moving forward.

# File names
## Script

When images containing images of barcoded specimen labels are saved to one of the `TO_PROCESS` folders in [Google Drive]({{ site.baseurl }}/documetation/imaging/#google-drive), they will be renamed and reorganized overnight. Please thoroughly review the documentation on the barcode reading [script](https://github.com/LACMIP/imaging) for more information on how to implement this step of the imaging workflow.

## Keystroking
Avoid manually renaming files whenever possible. However, sometimes file names must be hand keystroked. File names should conform to this format:
   `LACMIP_cat#_Genus_species_etc`

Images containing barcodes can be renamed using the barcode scanner, which acts like a keyboard. Scan the barcode in the image to insert the catalog number into the file name. However, the file name should still be manually altered to conform to the preferred format.

**Take care when naming images. If a catalog number is mistyped into a file name, the image will become disassociated from the correct specimen record.** Once the image is ingested into EMu, the DAMS, and picked up by aggregators, such errors can become very time-consuming to correct.
{: .notice--warning}

# Metadata
Images destined for EMu and the web should have metadata applied to them in Adobe Bridge. To do so, open Adobe Bridge and navigate to the folder containing the images you'd like to append metadata to. Select all images in the folder, then choose _Tools > Append Metadata_, and select the desired template. (Do not choose _Replace Metadata_.) The first time you do this, you may need to load your desired metadata template into Bridge: _LACMIP Imaging > Imaging Templates_.

If you are applying metadata to images _after_ they have been uploaded to Google Drive, this step will be most easily accomplished using Finder and the desktop version of Google Drive for Mac.

{% include figure image_path="/assets/images/imaging_metadata.png" alt="How to apply metadata to images in Bridge" caption="**Figure illustrating how to apply metadata to images in Adobe Bridge.** Right-click the image above to enlarge it in a separate tab or window." %}
