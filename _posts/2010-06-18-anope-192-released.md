---
layout: post
title: Anope 1.9.2 Released
author: chaz
category: 2010
# date: 2010-06-18T20:48:38+00:00
---

The Anope Team are pleased to announce the release of Anope 1.9.2.

This release brings a number of improvements since 1.9.1-p1, major highlights such as:

Removed binary databases in favour of flat file plaintext ones.
<br/>
Modestacker to combine mode changes together.
<br/>
Chanserv persist to keep services bots in channels when channel is empty.
<br/>
IPv6 Link Support.
<br/>
Ability for anope to reconnect if the connection to the uplink dies.
<br/>
Support for multiple simultaneous encryption methods.
<br/>
InspIRCd 2.0 support

Live updating SQL and ability to execute commands through SQL which are reflected by Anope in its own databases. (This does not mean you can randomly edit the Anope SQL Tables, you use the commands table to send 'normal' anope commands which anope interprets and updates both sets of databases with)

This will be further developed/re-engineered in 1.9.3 but it's a good start.

*IMPORTANT NOTE* - MySQL Support does not function properly within Windows in this release, it will be provided in 1.9.3.

As always, we encourage early adopters of development releases to exercise caution and take frequent system back ups knowing full well it might destroy your plans on a Friday night. We have been running 1.9.2 on Teranova for some time now and only uncovered a few unseen bugs. (This was on both Unreal and subsequently our migration to InspIRCd 1.2).

In order to convert your databases to the new 1.9.2+ format you must run the db-converter executable which will generate anope.db

To compile MySQL support in this version you will require mysql++ and to copy the modules from modules/sql to modules in the anope source.

We are developing a php web solution which will feature shortly allowing users to modify their own details from your website. We welcome suggestions on our forum for functionality this could include.

MD5 Checksums (stored away from the files themselves)
<br/>
(Future releases may include further security measures such as GPG/etc)

MD5: dd44ae0909083e7aab6e75f0d621269f  <a href="https://sourceforge.net/projects/anope/files/anope-devel/Anope%201.9.2/anope-1.9.2-source.tar.gz/download">anope-1.9.2-source.tar.gz</a><br/>
MD5: 2351a176e84d8bb463e5b57f0fcc774f <a href="https://sourceforge.net/projects/anope/files/anope-devel/Anope%201.9.2/anope-1.9.2.exe/download">anope-1.9.2.exe</a><br/>

We have provided a diff stat to show just how much has changed between 1.9.1 and 1.9.2, you can view it <a href="https://www.anope.org/1.9.2.diff.txt">here</a><br/>

*UPDATE* - We have replaced the Anope-1.9.2.exe which is available for download following a bug being reported in defcon.
