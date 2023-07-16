---
layout: post
title: Anope 1.8.5 Released
author: chaz
category: 2011
# date: 2011-02-06T16:01:46+00:00
---

The Anope Team is pleased to announce the immediate availability of Anope 1.8.5 (Stable) which introduces InspIRCd 2.0 support and refines the support of earlier versions.

Other noteable changes include:

* Support for building on MS Visual Studio 2010 (we still build the binary releases on VS2008)

* Improved logging facilities.

* Optional mail forking (for non Windows OS)

* Many many bug fixes (encourage all users to upgrade once tested)

As always we encourage all users of the stable branch to upgrade to the latest version when they are able to. Of course as per normal procedure you should run this on your testnet with your modules & databases before going live.

Finally, I write with some disappointment at the poor show of people willing to test this release. .

Too few people were willing to help us test this release which has delayed things considerably even to the point where I wasn't going to bother until people actually did take part. I then decided this was unfair to those who did bother and to that end here it is.

My thanks as always go to the folks who did bother; you guys know who you are and we're grateful for your continued support.

We would welcome more support in the future to avoid potential release delays. Contact me if you are interested.

<b>Changelog:</b>

05/05  A Added an internal event called when a nick is requested         [  #00]
<br/>
05/09  A Added an Atheme to Anope database converter                     [  #00]
<br/>
05/12  A Added logging for stateful commands                             [  #00]
<br/>
05/22  A Added an internal event called when a nick is ghosted           [  #00]
<br/>
05/22  A Added an internal event called when a nick is recovered         [  #00]
<br/>
05/23  A Added old nick parameter to EVENT_CHANGE_NICK                   [  #00]
<br/>
08/13  A Added forking for mail sending on supporting operating systems  [  #00]
<br/>
09/05  A Added InspIRCd 2.0 support                                      [  #00]
<br/>
04/15  F Fixed os_info to backup its database on Windows                 [  #00]
<br/>
04/15  F Fixed a potential crash in cs_clear ops when using UnrealIRCd   [#1154]
<br/>
04/16  F Fixed missing TS6SID on FJOIN in inspircd12                     [  #00]
<br/>
04/19  F Fixed ns_info to show nick expire times to opers not only admins[  #00]
<br/>
04/28  F Fixed a bug that could make some nick requests disappear        [  #00]
<br/>
05/18  F Fixed English and grammar in e-mail messages                    [  #00]
<br/>
05/23  F Fixed SQUITing juped servers on InspIRCd 1.2                    [#1165]
<br/>
06/15  F Fixed ./Config to correctly load config.cache                   [  #00]
<br/>
06/24  F Fixed pseudo-client kills not being detected on some TS6 IRCDs. [  #00]
<br/>
07/01  F Fixed encrypting very long passwords when registering           [#1172]
<br/>
08/03  F Fixed tracking users vhosts when there is no vhost mode         [#1178]
<br/>
08/05  F Fixed tracking of our clients after nick changing on InspIRCd   [#1180]
<br/>
09/10  F Fixed pseudo-clients always getting oper on InspIRCd.           [  #00]

Provided by Han` <Han@mefalcon.org> - 2010
<br/>
8/14   F Updated german language file.                                   [  #00]


<b>Files:</b>

<a href="https://sourceforge.net/projects/anope/files/anope-stable/Anope%201.8.5/anope-1.8.5.tar.gz/download">anope-1.8.5.tar.gz</a> - c876b7b7cda916faecfb78068121df02

<a href="https://sourceforge.net/projects/anope/files/anope-stable/Anope%201.8.5/Anope-1.8.5.exe/download">Anope-1.8.5.exe</a> - 8c33d0b00bac7e9f48ef18123ca36448

<a href="https://sourceforge.net/projects/anope/files/anope-stable/Anope%201.8.5/Anope-1.8.5-MySQL.exe/download">Anope-1.8.5-MySQL.exe</a> - 9d084c37486adcd74f1da42ff68d6d6b
