---
layout: post
title: Anope 1.9.3-p1 & Anope 1.9.4 Releases
author: chaz
category: 2011
# date: 2011-05-16T09:44:42+00:00
---

The Anope Team are pleased to announce the release of two development builds.

Firstly, 1.9.3-p1 which is a patch release of 1.9.3 with fixes/etc for that particular branch and then a release of 1.9.4 which has the fixes from 1.9.3-p1 where appropriate together with heaps more development on top.

Admins running 1.9.3 at the moment have two choices, update to 1.9.3-p1 as a small upgrade to improve the stability of 1.9.3 (but it's still dev!), or upgrade to 1.9.4 which carries larger risks as this branch has received much more development but has lots more new shiny features for you to play with.

We make these releases available to you to help find issues and improve the stability whilst we continue to drive the direction of development forward.

We welcome admins to try these releases and find bugs and suggest improvements but please be aware that these are not to be considered stable so do not complain if they crash and burn or eat your dinner.

We continue to make great progress on the development of Anope and once again I take my hat off to the team and especially to Adam for the time and effort he puts into this product. He is clearly a master of the <a href="https://xkcd.com/320/">28 hour day</a>.


<b>Changes in 1.9.3-p1</b>
F Fixed bad logic in /os exception preventing valid hosts from being added
<br/>
F Fixed /os sqline clear
<br/>
F Fixed not applying SQLines to our own clients
<br/>
F Fixed crash from deleting nonexistant users on the XOP access lists
<br/>
F Fixed crash when /cs set mlock is given an empty string
<br/>
F Fixed a potential crash from expiring nicks
<br/>
F Fixed build on Debian Lenny
<br/>
F Fixed /bs badword del to show what word was deleted
<br/>
F Fixed using /ns release with a password
<br/>
F Fixed allowing setting a valid TTB with /bs kick repeat
<br/>
F Fixed caps kicker
<br/>
F Fixed many SQL issues
<br/>
F Fixed reading resolv.conf if it has multiple spaces or tabs
<br/>
F Fixed creating permanent channels on burst and setting their topics
<br/>
F Fixed /cs register to show in HELP
<br/>
F Fixed restricting people from registering guest nick names
<br/>
F Fixed a potential crash from dropping nicks

<b>Changes in 1.9.4</b>

A Automatically set channel founder to the user with the highest access if there is no successor
<br/>
A /chanserv clone command to copy settings from one channel to another.
<br/>
A /chanserv mode command
<br/>
A Ability for users to delete their own access in channels
<br/>
A Added support for Plexus 3
<br/>
A Readded in support for /cs op/deop/etc to op/deop you in all channels
<br/>
A Added LDAP support
<br/>
A Added live SQL support
<br/>
A Added support for learning tracking/storing/locking all modes at runtime
<br/>
A Added m_alias
<br/>
A Added support for XMLRPC queries
<br/>
A Added /botserv set msg
<br/>
A Added /operserv config
<br/>
A Added /ns cert
<br/>
A Added /operserv login
<br/>
F Changed the GHOST command to not allow ghosting unidentified users if the RECOVER command exists
<br/>
F Some failed logic in /operserv exception that prevents proper exceptions from being added
<br/>
F Fixed the anope_os_sxlines MySQL table and code to work after restarting


<b>Files:</b>

1.9.3-p1

MD5 Sum: 168de16417f3489b2e492920c4bd9b42  <a href="https://sourceforge.net/projects/anope/files/anope-devel/Anope%201.9.3-p1/anope-1.9.3-p1-source.tar.gz/download">anope-1.9.3-p1-source.tar.gz</a><br/>
MD5 Sum: 23a91a1b8d27970fd0b8e1e9a2be9c75  <a href="https://sourceforge.net/projects/anope/files/anope-devel/Anope%201.9.3-p1/anope-1.9.3-p1.exe/download">anope-1.9.3-p1.exe</a><br/>

1.9.4

MD5 Sum: 41178aa1aa52038316bb1e6e02d93f07  <a href="https://sourceforge.net/projects/anope/files/anope-devel/Anope%201.9.4/anope-1.9.4-source.tar.gz/download">anope-1.9.4-source.tar.gz</a><br/>
MD5 Sum: e631f1c2becd56cd0f9a8f52afa934dd  <a href="https://sourceforge.net/projects/anope/files/anope-devel/Anope%201.9.4/anope-1.9.4.exe/download">anope-1.9.4.exe</a><br/>
