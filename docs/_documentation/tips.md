---
title: Tips
navcat: Basics
tags:
---
See the [Keyboard Shortcuts & Quick Reference Guide](http://help.emu.axiell.com/latest/en/Resources/Downloads/Quick%20Reference%20Guide/EMu_QuickRef_Guide_IE_20170629.pdf) from Axiell.

[Finding a field](http://help.emu.axiell.com/latest/en/Topics/Common/Find%20a%20field.htm) can be difficult.

## Improving EMu's performance

If EMu is responding very slowly, try a simple adjustment to your search options. You may have come across a situation where a search is taking a very long time and you just want to abort it and try different parameters. These changes should help with that.

Right-Click anywhere on Command Center (where to modules are displayed), and select “Options.” Select the SEARCHING tab and change these fields, then click OK
Maximum search time: place a number in here, do not leave it as zero. Your discretion. The example below is set to 4 minutes (240 seconds).
Maximum records retrieved: You may leave this as 0, but you may adjust this if it makes sense for you or a particular search.
Update search count every: change to 0 if you don’t want EMu to dedicate any resources bothering with this. Or set a high number if you want EMu to spend fewer resources.

Finally, if a search surpasses your Maximum Search Time, a message will appear:

This next option may take a bit of experimentation to find the optimal settings. Also, using these options means EMu starts slower, but once opened, performs better.

Right-Click anywhere on Command Center (where to modules are displayed), and select “Options.” Select the MODULES tab and change fields, then click OK. Double-click a module name (or click and select Change) : e.g. Catalog

Cached at Startup: start with 1. This sets the number of forms of that module that are cached for fast retrieval. The more you cache, the more RAM is used. You may not need more than 1. Try setting Catalog, Sites, and maybe Bibliography and Multimedia. Again, experiment with this.
Maximum Cached: As forms are opened, how many do you want cached. Again, I’d start with a low number (1 or 2) and then experiment with other settings.
Read Module Schema on Startup: this definitely slows EMu startup, but it may help significantly once EMu is running.

EK set "Cached at Startup" and "Maximum Cached" to 1 each for the Catalogue, Sites, and Taxonomy modules, and checked the box for "Read Modules Schema on Startup." Start up definitely takes longer (1.5 to 2 minutes vs. 1-3 seconds) but that's not a big deal if the performance once EMu is running is significantly better, which it is!

Problem prior (2018-11-03) to the above fix: Attaching and deleting records takes a significant amount of time. I've been test cataloging directly in EMu and on average (with the new default values you added for us--thanks!) one basic record takes 35 seconds. A third of those 35 seconds is spent waiting for EMu to attach the Site record (6 seconds), and attach the Taxonomy record (6 seconds). Worse, deleting a record takes 3-5 minutes.
