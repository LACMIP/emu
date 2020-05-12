---
title: Associating Records
navcat: Workflows
tags: cataloging
last_modified_at: 2019-12-05
---

Specimens that are physically stuck together but represent different taxa must be cataloged separately (e.g., when a bivalve and gastropod are preserved on the same rock, or when a trace fossil is found on a body fossil). These records must be associated using the [*Relationships* tab](https://lacmip.github.io/emu/documentation/catalogue/) in the Catalogue module.

## Workflow for associating specimen records

*1.* Once you have cataloged all specimens to be associated, open a second instance of the Catalogue module.
{% include figure image_path="/assets/images/catalogue_relationships1.png" alt="screenshot of the Relationships tab in the catalogue module" %}

*2.* In the new instance of the Catalogue module, search for all records to be associated.
{% include figure image_path="/assets/images/catalogue_relationships2.png" alt="screenshot of the Relationships tab in the catalogue module" %}
{% include figure image_path="/assets/images/catalogue_relationships3.png" alt="screenshot of the Relationships tab in the catalogue module" %}

*3.* In the original instance of the Catalogue module, open one of the specimen records and navigate to the *Relationships* tab.

*4.* Select all records to be associated in the second instance of the Catalogue module. Drag them into the *Related Records* fields on the first specimen record.

*5.* **Circular relationships should be avoided.** Therefore, delete the row in the _Related Records_ table that references the specimen record you are actively working on.

*6.* Save this change and :repeat:repeat steps 3-5:repeat: for all other specimen records that need to be associated.

{% include figure image_path="/assets/images/relationships_assocspmsexample.png" alt="Example of a catalog record that is associated with other records." caption="If a relationship is created between two or more Catalogue records, an icon will appear in the summary line." %}
