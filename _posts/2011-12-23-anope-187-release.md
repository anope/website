---
layout: post
title: Anope 1.8.7 - Release
author: Adam
category: 2011
# date: 2011-12-23T23:12:20+00:00
---

The Anope Team are pleased to announce the immediate availability of Anope IRC Services 1.8.7 which contains a small number of changes including support for Hybrid channel modes +S and +O & additional internal events for certain situation offering flexibility to Module Authors.

The small number of bug fixes in this 7 month period since the last 1.8 release goes a long way to show how stable Anope 1.8 has and continues to be for the community.

This release is recommended for all networks running earlier 1.8 releases and as always we recommend taking a good back up and testing your modules and database in a testing environment before upgrading.


<b>Change Log:</b>

08/18 A Added support for Hybrid's channel mode +S [#1319]
<br/>
08/18 A Added support for Hybrid's channel mode +O [#1320]
<br/>
08/21 A Added internal event when a nickcore is dropped. [ #00]
<br/>
08/21 A Added internal event when a nickcore gets a new display nick. [ #00]
<br/>
08/18 R Removed support for Hybrid's (old) channel mode +a [#1318]
<br/>
12/15 C Added API support for SVSJOIN and SVSPART on UltimateIRCd 3. [ #00]
<br/>
05/30 F Fixed removing vhosts on InspIRCd when m_cloaking is unloaded [#1273]
<br/>
07/23 F Fixed a potential crash in the badwords kicker [ #00]
<br/>
08/09 F Fixed deopping the first user to join a channel during a burst [#1287]
<br/>
08/10 F Fixed loading bs_fantasy_owner on InspIRCd 2.0 on startup [ #00]
<br/>
08/21 F Send DROP event when forbidding nicks and channels. [ #00]
<br/>
11/16 F Fixed ident being used instead of vident in some comparisons. [ #00]
<br/>
11/20 F Fixed ignore not matching against users' real host or IP. [ #00]
<br/>
12/06 F Fixed some typos in the spanish language file [ #00]


<b>Files:</b>

MD5: ef28b940d58924693f62296c9e306ac9 <a href="https://sourceforge.net/projects/anope/files/anope-stable/Anope%201.8.7/anope-1.8.7.tar.gz/download">Anope-1.8.7.tar.gz</a><br/>
MD5: 71666440eba4305a80be4474414f5959 <a href="https://sourceforge.net/projects/anope/files/anope-stable/Anope%201.8.7/Anope-1.8.7.exe/download">Anope-1.8.7.exe</a><br/>
MD5: 0e5352e1b6805300340126250c767318 <a href="https://sourceforge.net/projects/anope/files/anope-stable/Anope%201.8.7/Anope-1.8.7-MySQL.exe/download">Anope-1.8.7-MySQL.exe</a><br/>
