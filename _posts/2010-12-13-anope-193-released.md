---
layout: post
title: Anope 1.9.3 Released
author: chaz
category: 2010
# date: 2010-12-13T17:56:21+00:00
---

We're pleased to announce the release of Anope 1.9.3 (Development). This release continues the development of our development branch in creating the next generation Anope 2.0 stable.

Specific changes in this release include:

Added SSL Support for connections(*)
<br/>
Added threading support for mail sending
<br/>
Added a DNS blacklist system & asynchronous DNS system
<br/>
Added a new language system that uses gettext
<br/>
Added m_mysql which uses threads to execute queries
<br/>
Increased flexibility in a new logging system
<br/>
+ stability & bug fixes

As always we welcome early adopters to the development branch to enable us to focus development and functionality moving forward but of course please do take back ups if you intend on trying this version out and be aware that you can not take databases from 1.9 back to 1.8 stable.

Admins moving from 1.9.2 will need to ensure they run their databases through db-upgrade to ensure they move to the new database format.

Advice is available in #anope on irc.anope.org

* The precompiled Windows releases lack SSL support due to licensing limitations but please read docs/WIN32.txt for information on compiling your own Anope from source if you need this functionality. We are working on ways to make this process smoother moving forward.

MD5 Checksums

anope-1.9.3-source.tar.gz - 89e7c887f4644a61b514d903f3e86b84

anope-1.9.3.exe - a23cb196b624bd942870414b1ba065d4

<a href="stat192-193.diff">diffstat between 1.9.2 and 1.9.3 </a><br/>
