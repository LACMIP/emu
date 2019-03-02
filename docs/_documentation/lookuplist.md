---
title: Lookup Lists
navcat: Modules
tags:
last_modified_at: 2019-03-01
---
The Lookup Lists module is where lookup list values are managed. **Generally, staff do not need to use this module**, as they should have permission to add values to a lookup list while editing a record, e.g. while entering a new county in the *County/Dist* field. Students may not have permission to do so, and in this case a staff member would need to add the value for them. **Staff do need to use the Lookup List module to add values to drop-down menus.** For general information about this module, please see [Axiell's documentation](http://help.emu.axiell.com/latest/en/Topics/Common/Lookup%20Lists%20module.htm).

{% include figure image_path="/assets/images/lookuplist_example.png" alt="image of EMu lookup list for geologic age" caption="Lookup lists help us maintain consistent data by autofilling common information. For example, if you are editing the Site record above and you enter data into EMu's *Age* field, that field is linked to a lookup list that knows the hierarchy of our geologic time data. When you enter 'Turonian' in *Age*, Emu automatically fills the fields for *Epoch* and *Period*." %}

Lookup lists are built “on the fly” by EMu, and this process is managed by the Lookup Lists module. EMu tries to strike a balance between being flexible and maintaining data quality through the use of **"persistent"** vs. **"non-persistent"** lookup list values. Lookup list values that are entered by users, a la the *County/Dist* example in the first paragraph, are by default not persistent and will delete themselves if no records are using them. Persistent lookup list values are those that should *always* appear as an option, regardless of whether or not they are in use. An example of persistent lookup list values are those in the Catalogue record field for *Collection*.

## Finding a lookup list

EMu fields that are linked to lookup lists are usually indicated by an icon that looks like three bars and an arrow, to the right of the field. Fields with dropdown menus are also linked to lookup lists. In order to find a lookup in the Lookup Lists module, you need to know the name of the list, which is often similar but not the same as the name of the field. Use the question mark tool in the upper right of any module to click inside the field for which you want to find the lookup list. A new window will pop up, as shown in the figure below. Copy or take note of what is listed next to *Lookup Name*; you will use this within the Lookup List module.

{% include figure image_path="/assets/images/lookuplist_findname.png" alt="screenshot of how to find the name of a lookup list" caption="Screenshot of the EMu Sites module, illustrating how to use the question mark tool to see the lookup list name for any field which has one." %}

Open the Lookup List module and paste or type your *Lookup Name* into the search for *Lookup List Name*. This will bring up all lookup values that belong to this list.

{% include figure image_path="/assets/images/lookuplist_lithostratigraphic.png" alt="screenshot of search results for the Lithostratigraphic lookup list" caption="Lookup List module search results for the 'Lithostratigraphic' lookup list name. Notice that values can have multiple levels, which in this lookup correspond to *Formation* and *Member*." %}

## Adding values to a lookup

You may need to add values to a lookup list if it populates a dropdown menu, or if you want to prepare for student users who don't have permission to add values as they edit. To do so, find the appropriate lookup list, as described above. Open one of the records for reference and **make sure you understand what each level of value means for your data**.

{% include figure image_path="/assets/images/lookuplist_addvalue.png" alt="screenshot of a Lookup List record" caption="The example Lookup List record here belongs to the Lithostratigraphic lookup, and each level corresponds to a lithostratigraphic hierarchy: group, formation, and member. Not all formations belong to a group in LACMIP data, and therefore the first level has no value." %}

Leave the example record open while also opening a new Lookup List record. Enter the *Lookup List Name*, and values for whatever levels are appropriate. Choose for the record to be either persistent or non-persistent (most of the time if you are going to the trouble of adding a lookup list record, you'll want it to be persistent). You should only edit fields on the first tab (*Lookup 1*) of this module. Keep in mind that while LACMIP staff have permission to add values, they cannot edit the content of values. For this reason, it is important to check your work and make sure spelling, etc. is correct before you save the new Lookup List record.

You can also add values to the Lookup Lists module in bulk via a CSV file. Please contact the Museum's database manager if you are interested in this option.

## Cleaning up values in a lookup

The only thing LACMIP staff can edit on a Lookup List record after it has been saved is whether the record is persistent or not. **Changing a record from persistent to non-persistent means that any records whose values are not being used by records in other modules will disappear.** This is the only way to clean up values via the Lookup List module. If you want to clean up the content of values, e.g. fix all instances of "Warley Hill Fm." to be "Warley Hill Formation", this needs to be done in the data itself (see documentation for [Global Replace](http://help.emu.axiell.com/latest/en/Topics/Common/Global%20Replace.htm)). The Lookup List module will rebuild itself and automatically fix values that are fixed in the data.

To reiterate, cleaning up values in the Lookup List module **does not** clean up values that exist on any individual record. However, changing *Persistent* to "No" for a particular Lookup List record, then replacing those values in your Catalogue/Sites/etc. module will remove the offending Lookup List record. Check with the Museum's database manager if you need help cleaning up lookup lists.
