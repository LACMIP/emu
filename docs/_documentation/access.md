---
title: Accessing EMu
navcat: Basics
tags: cataloging georeferencing quick-start taxonomy
last_modified_at: 2019-02-01
---

EMu is software that is hosted on an internal server and runs on your desktop. The Museum's database manager (Bill Mertz) is responsible for maintaining this system and for providing access.

## User accounts

Every person who uses EMu should have their own account, and even temporary users (e.g. students) should never share an account. This is because EMu tracks user actions with an audit trail, which allows an administrator to see exactly who was involved if a problem exists. To request a new account, send the full name of the new user to the Museum’s database manager.

It is important to only request accounts for users who will actively use EMu, and to tell the database manager when an account should be closed. We track LACMIP non-staff accounts in a spreadsheet called *EMu_LACMIP-Users.xlxs* in the folder *Dropbox > EMu > Admin*.
{: .notice--warning}

## Logging in & out

To log in to EMu, open the program and enter your username and password. You will also need to enter data for host (“kemu”) and service (“emulacm”). It is very important that when you are done using EMu you shut down the program. The Museum pays for a certain number of licenses, which means that only an amount of users equal to the number of licenses can use EMu at any given time.

## Remote access

Users can access EMu offsite from the Museum (e.g. at the LACMIP warehouse) via the Marconi server. Marconi connects you to a remote desktop at the Museum, which runs the actual EMu software. You will need to log in to the Museum's VPN before you can complete the EMu login process described above.

To log in remotely, go to [https://vpn.nhm.org](https://vpn.nhm.org) and enter your username and password. If you are a full-time staff member, you should be able to use the same credentials as you use for your email (if not, ask IT to set you up with VPN access). For part-time staff, interns, and volunteers, IT has created four generic VPN logins for LACMIP to use. The usernames and passwords for these accounts can be found in a spreadsheet called *EMu_LACMIP-Users.xlxs* in the folder *Dropbox > EMu > Admin*.

Once logged in, at the bottom of the page you should see a link to **“Terminal Server (MARCONI).”** Clicking on this will run Marconi in your browser. Once Marconi is running, you will see a remote desktop from which you can open the EMu application. When you are done using Marconi, exit by clicking the door icon in the upper right toolbar. Marconi will automatically log you out after two hours for security purposes, but when it does so any applications you were running on the remote desktop will remain open (so you won’t lose anything, you’ll just need to log in again).

To transfer files into the remote desktop, drag and drop them. You will see a status bar in the lower right corner of the window, and once the file has uploaded you can find it in the *G on Guacamole RDP* folder of the computer. To transfer files from the remote desktop to your local computer, drop them into the the folder *G on Guacamole RDP > Downloads.*

## User Permissions

LACMIP full-time staff should have rights to create, edit, and delete [Catalogue]({{ site.baseurl }}/documentation/catalogue/), [Multimedia]({{ site.baseurl }}/documentation/multimedia/), [Bibliography]({{ site.baseurl }}/documentation/bibliography/), [Site]({{ site.baseurl }}/documentation/sites/), and [Taxonomy]({{ site.baseurl }}/documentation/taxonomy/) records. Staff can create [Lookup]({{ site.baseurl }}/documentation/lookuplist/) and [Transaction]({{ site.baseurl }}/documentation/transactions/) records, but not delete or edit them. Staff can only view [Accession]({{ site.baseurl }}/documentation/accessions/) and [Party]({{ site.baseurl }}/documentation/parties/) records.

Permissions for LACMIP part-time staff, interns, and volunteers can be set on a case-by-case basis by the Museum's database manager.

## Sharing

Data in all modules is shared by everyone with access to the Invertebrate Paleontology collection in EMu.

Reports and lists created by one user may be shared with other users if the creator so chooses. If a list or report is shared, only the owner can edit it. However, a shared user can copy the original report/list to create their own which they can then edit. Shared lists do not disappear from other users when the user who created them has their account closed.

## Mac vs. PC

EMu can only be used on a Mac computer via remote access (above) or a virtual simulator such as Parallels or VMWare. Remote access is slightly different on a Mac versus a PC. Certain features, such as copy-pasting between your local desktop and the remote desktop, do not work but the general functionality is equivalent. For key commands, remember to use the "ctrl" key vs. the "command" key.
