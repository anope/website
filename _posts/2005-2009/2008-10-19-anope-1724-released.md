---
layout: post
title: Anope 1.7.24 Released
author: chaz
category: 2008
# date: 2008-10-19T19:40:47+00:00
---

Following the successful release of 1.7.23b we are pleased to announce the release of 1.7.24 which has a few language file fixes and an important MySQL change see below.

** Important - MySQL **

It is crucially important that if you use MySQL with UseRDB that you for the first time running 1.7.24 disable UseRDB, start up anope from Flatfile DBs and perform an /OS UPDATE to dump the data into your MySQL Database before shutting down and enabling UseRDB.

This is due to a change in the way passwords are stored in MySQL and therefore we are keen to hear from users if you run into any problems and cannot recommend strongly enough that you take a back up prior to upgrading!

***

We are edging closer to the release of 1.8!

Check out the <a href="https://sourceforge.net/project/shownotes.php?group_id=94081&release_id=634471">Change Log</a> Here. 

Files:

anope-1.7.24.tar.gz -- Full 1.7.24 source release
<br/>
anope-1.7.24.exe -- Windows Installer (No MySQL Support)
<br/>
anope-1.7.24-mysql.exe -- Windows Installer (With MySQL Support)

MD5:

3c956362b4b4d074e2e58c869c77f77c *anope-1.7.24.tar.gz
<br/>
153b45b56f16b0081db6af132e50b7c7 *anope-1.7.24.exe
<br/>
40626071e74bf45629fe4cd8160f4f9f *anope-1.7.24-mysql.exe
