---
layout: post
title: Anope 1.8.6 - Release
author: Adam
category: 2011
# date: 2011-06-14T23:48:52+00:00
---

<!--
BEGIN SUMMARY
The Anope Team is pleased to announce the release of Anope 1.8.6 (Stable) which contains lots of general bug fixes and improved support for Plexus, & Hybrid IRCds.

This release only contains an updated German Language File (thanks Han!) and many Mac specific fixes both for compilation and indeed running of Anope on Mac.

I am somewhat disappointed once again at the lack of interest from people willing to test the releases despite ~100 downloads a day.


<b>Changelog</b>

10/31  A Added support for plexus3's channel mode +z                     [#1202]
<br/>
02/23  A Added account tracking support to ratbox protocol module        [  #00]
<br/>
03/21  A Added support for Hybrid's m_services and m_change              [  #00]
<br/>
03/28  A Added internal events called when a module is loaded/unloaded.  [  #00]
<br/>
03/28  A Added internal events called when a command is added/deleted.   [  #00]
<br/>
09/11  F Fixed db-convert handling some vhost collisions                 [  #00]
<br/>
09/14  F Fixed ./configure failing with partial SQL installations        [  #00]
<br/>
09/28  F Fixed ForkForMail to always work                                [  #00]
<br/>
09/28  F Fixed /nickserv saset display to use nicktracking if enabled    [#1193]
<br/>
09/28  F Fixed /nickserv group to use nicktracking if enabled            [#1194]
<br/>
12/12  F Remove vhost requests from nicks that expire                    [  #00]
<br/>
12/15  F Fixed /cs enforce #channel to say SET was enforced not (null)   [#1213]
<br/>
12/23  F Fixed /cs (un)ban and akick from matching users real hosts/IP   [#1079]
<br/>
01/19  F Fixed 'make install' recompiling src/tools                      [#1227]
<br/>
01/21  F Fixed many incorrect apostrophe usages                          [#1223]
<br/>
01/28  F Fixed not introducing our clients with usermode k on InspIRCd2.0[  #00]
<br/>
01/29  F Updated german language file.                                   [  #00]
<br/>
02/05  F Fixed wiki URLs in Windows configure script                     [  #00]
<br/>
02/11  F Fixed build on Mac                                              [  #00]
<br/>
02/23  F Fixed rejoining our clients if they are kicked on a TS6 IRCd    [  #00]
<br/>
03/02  F Fixed showing SENDPASS in HELP to users who can't use it        [  #00]
<br/>
03/03  F Fixed opping our clients on ratbox when not using TS6           [  #00]
<br/>
03/04  F Fixed setting a users host in InspIRCd when vhost is turned off [  #00]
<br/>
03/24  F Fixed groups display nick showing in HS req memos for aliases.  [#1252]
<br/>
04/28  F Fixed missing NS REGISTER reply when ns_register is not loaded. [#1263]
<br/>
05/02  F Fixed crash in enc_md5 on Mac                                   [#1236]

<b>Files:</b>

924338d39daa78947670c6c19023cc14 *<a href="https://sourceforge.net/projects/anope/files/anope-stable/Anope%201.8.6/anope-1.8.6.tar.gz/download">anope-1.8.6.tar.gz</a><br/>
d6b2bc0ac1393a01db63691c30a1a59e *<a href="https://sourceforge.net/projects/anope/files/anope-stable/Anope%201.8.6/Anope-1.8.6.exe/download">Anope-1.8.6.exe</a><br/>
73712ecd654731610ce1ddeaecc4687c *<a href="https://sourceforge.net/projects/anope/files/anope-stable/Anope%201.8.5/Anope-1.8.5-MySQL.exe/download">Anope-1.8.6-MySQL.exe</a>
END SUMMARY
-->

The Anope Team is pleased to announce the release of Anope 1.8.6 (Stable) which contains lots of general bug fixes and improved support for Plexus, & Hybrid IRCds.

This release only contains an updated German Language File (thanks Han!) and many Mac specific fixes both for compilation and indeed running of Anope on Mac.

I am somewhat disappointed once again at the lack of interest from people willing to test the releases despite ~100 downloads a day.


<b>Changelog</b>

10/31  A Added support for plexus3's channel mode +z                     [#1202]
<br/>
02/23  A Added account tracking support to ratbox protocol module        [  #00]
<br/>
03/21  A Added support for Hybrid's m_services and m_change              [  #00]
<br/>
03/28  A Added internal events called when a module is loaded/unloaded.  [  #00]
<br/>
03/28  A Added internal events called when a command is added/deleted.   [  #00]
<br/>
09/11  F Fixed db-convert handling some vhost collisions                 [  #00]
<br/>
09/14  F Fixed ./configure failing with partial SQL installations        [  #00]
<br/>
09/28  F Fixed ForkForMail to always work                                [  #00]
<br/>
09/28  F Fixed /nickserv saset display to use nicktracking if enabled    [#1193]
<br/>
09/28  F Fixed /nickserv group to use nicktracking if enabled            [#1194]
<br/>
12/12  F Remove vhost requests from nicks that expire                    [  #00]
<br/>
12/15  F Fixed /cs enforce #channel to say SET was enforced not (null)   [#1213]
<br/>
12/23  F Fixed /cs (un)ban and akick from matching users real hosts/IP   [#1079]
<br/>
01/19  F Fixed 'make install' recompiling src/tools                      [#1227]
<br/>
01/21  F Fixed many incorrect apostrophe usages                          [#1223]
<br/>
01/28  F Fixed not introducing our clients with usermode k on InspIRCd2.0[  #00]
<br/>
01/29  F Updated german language file.                                   [  #00]
<br/>
02/05  F Fixed wiki URLs in Windows configure script                     [  #00]
<br/>
02/11  F Fixed build on Mac                                              [  #00]
<br/>
02/23  F Fixed rejoining our clients if they are kicked on a TS6 IRCd    [  #00]
<br/>
03/02  F Fixed showing SENDPASS in HELP to users who can't use it        [  #00]
<br/>
03/03  F Fixed opping our clients on ratbox when not using TS6           [  #00]
<br/>
03/04  F Fixed setting a users host in InspIRCd when vhost is turned off [  #00]
<br/>
03/24  F Fixed groups display nick showing in HS req memos for aliases.  [#1252]
<br/>
04/28  F Fixed missing NS REGISTER reply when ns_register is not loaded. [#1263]
<br/>
05/02  F Fixed crash in enc_md5 on Mac                                   [#1236]

<b>Files:</b>

924338d39daa78947670c6c19023cc14 *<a href="https://sourceforge.net/projects/anope/files/anope-stable/Anope%201.8.6/anope-1.8.6.tar.gz/download">anope-1.8.6.tar.gz</a><br/>
d6b2bc0ac1393a01db63691c30a1a59e *<a href="https://sourceforge.net/projects/anope/files/anope-stable/Anope%201.8.6/Anope-1.8.6.exe/download">Anope-1.8.6.exe</a><br/>
73712ecd654731610ce1ddeaecc4687c *<a href="https://sourceforge.net/projects/anope/files/anope-stable/Anope%201.8.6/Anope-1.8.6-MySQL.exe/download">Anope-1.8.6-MySQL.exe</a>
