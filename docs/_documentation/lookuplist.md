---
title: Lookup Lists Module
tags:
---

When creating lookup lists, checking the “not persistent” box means that unused values will disappear.

Lookup lists are edited “on the fly” by EMu.  If a Lookup List record has Persitent=NO, it will delete itself if no catalog/sites/etc records exist with that value.  Therefore, changing Persistent to NO for a particular Lookup List record, then replacing those values in catalog/sites/etc will automatically remove the offending Lookup List record.

You can either create a new Lookup List record and check persistent = Yes, then replace all offending values in Catalog/Sites/etc. with the new valule.  Or you can replace the old values with new ones directly in catalog/sites/etc. then go to the Lookup Lists Module and make that newly created lookup list record Persistent (if you want it to be, of course).

why is the above better than "go to the lookup list record and edit it, thereby fixing all Catalog/Sites/etc. records that use this list value"? It's certainly not as intuitive or efficient.

Because editing the Lookup List does NOT change the values in the Catalog/Sites/etc. records.  All it does is change the lookup list.  The Lookup List module is not an attachment module like Sites or Parties.  Also, the Lookup List constantly rebuilds itself based on what values it finds in Catalog/Sites.

In fact, changing the values in Catalog changes the Lookup List values, not the other way around.  In other words, you cannot get rid of a value in the Lookup List by deleting it or changing it in the Lookup list.  If that value exists in Catalog, the Lookup List will create a new Lookup List record and insert it back into the Lookup List.  However, deleting or changing values in Catalog will automatically change or delete them in the Lookup List.

The only way to keep the Lookup List from deleting an unused value is to change Persistent to YES.
[needs content]
