---
title: Tips
navcat: Basics
tags: quick-start
---
Below is a non-exhaustive collection of tips for using EMu.

## Useful links from Axiell

- The [Keyboard Shortcuts & Quick Reference Guide](http://help.emu.axiell.com/latest/en/Resources/Downloads/Quick%20Reference%20Guide/EMu_QuickRef_Guide_IE_20170629.pdf) has useful key commands that can help you use EMu more efficiently. Keep in mind that not all key commands work on a Mac and/or via the VPN remote access.
- Field names in EMu can be difficult because they are frequently re-used between modules. This help page goes over [finding a field](http://help.emu.axiell.com/latest/en/Topics/Common/Find%20a%20field.htm).

## Default settings

You can view and change your default settings by right-clicking anywhere on Command Center (where the modules are displayed), and selecting *Options*. The following are settings on the *General* tab that you may want to personalize:
- *Save Last Position*: EMu will remember where modules and the Command Center were displayed on your screen.
- *Save Last Size*: As above, but EMu remembers the modules’ last size.
- *Show Field Help in Module Window*: Displays field help at bottom. Useful only if you’ve added help info to your fields (which LACMIP mostly has not).
- *Refresh Changed Records*: You may want to uncheck this. If checked, and you have multiple instances open (e.g. two Catalogue modules open at once) EMu updates both instances when one is edited. This can take a long time if thousands of records are opened in both instances.
- *Only Refresh if Less than*: If the above is checked, try setting a small number here (example: 100). In this case, EMu will skip the *Refresh Changed Records* process on instances displaying more than 100 records.
- *Cache Registry Lookups*: This should **always** be checked.
- *Clear Cache button*: This is used to reset the registry without having to restart EMu.
- *Cache System Resources*: Leave unchecked. This option was developed for old operating systems.

## Improving EMu's performance

If you are using EMu over the VPN, it often performs slowly. This may be due to the speed & stability of your internet connection, the configuration of EMu, or a combination of both. The following adjustments may help.

### Switch from wireless to wired internet connection

All of the Mac computers at the LACMIP warehouse access the internet wirelessly, but can also be plugged directly in via Ethernet (and the right adapter). If you are having consistent trouble with VPN time-outs or EMu running slowly, try connecting to the internet directly this way. All of the PC desktops are wired already.

### Change your default caching settings in EMu

Changing your default caching settings in EMu affects the amount of time the program takes to start up, and may require experimentation to find the optimal balance between slower starting up and faster operations once EMu is running.
1. Right-click anywhere on Command Center (where the modules are displayed), and select *Options*.
1. Select the *Modules* tab and change the following fields for each module you'd like to affect, then click OK:
    - *Cached at Startup*: start with 1. This sets the number of forms of that module that are cached for fast retrieval. The more you cache, the more RAM is used. You may not need more than 1. Try setting Catalog, Sites, and maybe Bibliography and Multimedia.
    - *Maximum Cached*: try starting with a low number, like 1 or 2.
    - *Read Module Schema on Startup*: checking this box definitely slows EMu startup, but it may help significantly once EMu is running.

For people doing specimen cataloging, we recommend setting *Cached at Startup* and *Maximum Cached* to 1 each for the Catalogue, Sites, and Taxonomy modules, and checking the box for *Read Modules Schema on Startup*. Startup definitely takes longer (up to 1.5 or even 2 minutes vs. 1-3 seconds) but that's not a big deal if the performance once EMu is running is significantly better, which it is!
{: .notice--warning}

### Change your default search settings in EMu

This adjustment may help if you are having problems with searches taking a very long time.
1. Right-click anywhere on Command Center (where the modules are displayed), and select *Options*.
1. Select the *Searching* tab and change the following fields, then click OK:
    - *Maximum search time*: place a number in here instead of leaving it as zero. Four minutes (240 seconds) is a good amount of search time to start with. If a search surpasses this maximum search time, a message will appear asking whether or not you want to abort.
    - *Maximum records retrieved*: leave this as 0, or adjust to whatever amount makes sense for you or for a particular search.
    - *Update search count every*: change to 0 if you don’t want EMu to dedicate any resources to bothering with this, or set a high number if you want EMu to spend fewer (but still some) resources.
