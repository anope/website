---
layout: post
title: Anope 1.8.4 - Release
author: chaz
category: 2010
# date: 2010-04-05T13:18:48+00:00
---

UPDATED - 5th April 2010


We're pleased to announce the latest release of the Anope stable branch; 1.8.4.

This release brings a list of fixes generally, and some further compatibility with InspIRCd 1.2.

As always we recommend you test the new version out in a testnet environment with your database and third party modules before considering upgrading.

We are in the process of also adding the functionality to our modules site (https://modules.anope.org/) to 'mass' build modules for Windows each time there is a new release from us which should hopefully help Windows' users make decisions upon upgrading irrespective of whether the module author has produced a new dll for them.


Changelog:

3/10  A Added support for tracking permanent channels                    [  #00]
<br/>
3/24  A Added logging of deleting and clearing XOP access lists          [  #00]
<br/>
2/9   F Fixed marking halfops as deopped, stops unsetting modes by them  [#1136]
<br/>
2/18  F Fixed listing unconfirmed nicks with suspended nicks to SA+      [  #00]
<br/>
3/2   F Fixed a bug that could cause access entries to disappear         [  #00]
<br/>
3/13  F Fixed maximum hostname checking in HS SET and HS REQUEST         [#1138]
<br/>
3/13  F Fixed deleting force dropped nicks from the hs_waiting list      [#1139]
<br/>
3/13  F Fixed backing up 3rd party module databases more than once a day [#1140]
<br/>
3/16  F Fixed os_info to display syntax errors if no command is entered  [  #00]
<br/>
3/29  F Fixed defcon to only apply its mode parameters when it's on      [#1146]
<br/>
3/29  F Fixed numbering of memos when saved in SQL                       [#1149]
<br/>
3/30  F Fixed module demos to work correctly on TS6 IRCDs                [  #00]
<br/>
4/3   F Fixed saving databases in readonly mode when using anoperc       [  #00]

Files:

<a href="https://sourceforge.net/projects/anope/files/anope-stable/Anope%201.8.4/anope-1.8.4.tar.gz/download">anope-1.8.4.tar.gz</a> - MD5:75741c781b45e5e7e8588282aef97e35

<a href="https://sourceforge.net/projects/anope/files/anope-stable/Anope%201.8.4/Anope-1.8.4.exe/download">anope-1.8.4.exe</a> - MD5:cce75579749c8a1ad8779917bee61cd1

<a href="https://sourceforge.net/projects/anope/files/anope-stable/Anope%201.8.4/Anope-1.8.4-MySQL.exe/download">anope-1.8.4-MySQL.exe</a> - MD5:1bac90018f32c019d4dc1eaf7a77240f


In a fairly unusual move for us I'd like to dedicate this release to Adam as not only is he a development machine but he's a genuinely nice guy and we're very grateful for the time and effort he puts into the project. If anyone in the real world is looking for a young developer with an incredibly bright future get in touch; he's definitely worth your time.

On the roadmap for the near future we're in the middle of rewriting the socket system for 1.9.2, and having just introduced a SQL Interface which whilst not being "live SQL" as most will think this provides a sensible and easy to use commands table which Anope will process at intervals so you can in theory do anything via SQL that you could do from an IRC client and yes, this will open the doors to web system integration etc and we've provided a small php page to demonstrate this. (Usual warnings that trunk will probably eat your breakfast and make fun of your wife. Hint, do not use it in a production environment.)

It's busy times here and what with our friends over at InspIRCd working on 2.0 and 2.1 of their software we are predicting quite a productive year for IRC as a whole and that's something I'm sure we're all excited about and glad to hear. Onwards and upwards.

As always, if you are interested in helping / working with us in any way please do get in touch (chaz@anope.org), & thank you of course to our <a href="https://www.anope.org/sponsors.php">sponsors</a> for their selfless kindness.

Finally, Happy Easter to those who celebrate it.


Charles.


Update 5th April 2010
<br/>
- The autobuild functionality is now available within our Modules Site at <a href="https://modules.anope.org">https://modules.anope.org/</a> with a special thank you to LEthaLity for working with Adam on integrating the modules back into the system for this release. Cheers mate!
