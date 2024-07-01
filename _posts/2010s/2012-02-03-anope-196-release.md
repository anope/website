---
layout: post
title: Anope 1.9.6 - Release
author: Adam
category: 2012
# date: 2012-02-03T22:44:04+00:00
---

The Anope Team are proud to announce the release of Anope 1.9.6. This release continues the development of our development branch in creating the next generation Anope 2.0 stable.

Some configuration changes have been made, we recommend users upgrading start with a fresh configuration file.

A new database format has been added, and the old db_plain has been deprecated. Users upgrading should read the example configuration for instructions on how to upgrade their databases.
<br/>
As always, keep backups.

Users using MySQL with previous versions will need to export their databases to flatfile first before importing into 1.9.6.

Change log includes:

Anope Version 1.9.6
<br/>
--------------------
<br/>
A Added ability to configure emails sent by services
<br/>
A Added chanserv/up and chanserv/down
<br/>
A Added m_proxyscan
<br/>
A Added more configurability for what vhosts are valid
<br/>
A Added chanserv/log
<br/>
A Added ability to configure ChanServ privileges
<br/>
A Added a new database format
<br/>
A Added SQLite support
<br/>
A Added more verbose messages on startup
<br/>
A Added ability for chanserv/suspend and nickserv/suspend to take an expiry time
<br/>
A Added no nickname ownership config option
<br/>
A Added m_rewrite
<br/>
A Added akill IDs
<br/>
F Fixed crash in clearusers
<br/>
F Fixed crash in /os oper info
<br/>
F Fixed eventfd Config check to work properly on OpenVZ

MD5 Sum: cb2baa3f09da38a1f5064f1af09b6bf0 <a href="https://sourceforge.net/projects/anope/files/anope-devel/Anope%201.9.6/anope-1.9.6-source.tar.gz/download">anope-1.9.6-source.tar.gz</a><br/>
MD5 Sum: a4799b5bf5f3aa7da376923d60fe9e6d <a href="https://sourceforge.net/projects/anope/files/anope-devel/Anope%201.9.6/anope-1.9.6.exe/download">anope-1.9.6.exe</a><br/>
