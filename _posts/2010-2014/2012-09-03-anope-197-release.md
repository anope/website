---
layout: post
title: Anope 1.9.7 - Release
author: Adam
category: 2012
# date: 2012-09-03T08:22:16+00:00
---

The Anope Team are proud to announce the release of Anope 1.9.7. This release continues the development of our development branch in creating the next generation Anope 2.0 stable.

Some of the highlights include:

    Added regex support for many commands, such as akill, sqline, snline,
<br/>
    and all of the */list commands.

    Extended the ability of akill to match against a full nick!user@host and
<br/>
    real name of users.

	Added nickserv:registration configuration option to configure how new accounts are verified.
<br/>
	Added nickserv:unregistered_notice configuration option to send a custom message to unregistered users on connect.

	Added chanserv:require configuration option to set which modes must be on all registered channels.
<br/>
	 
<br/>
	Added options:casemap configuration option to choose how case insensitive strings are compared, using ASCII, rfc1459, or a locale installed on the system.
<br/>
	
    db_sql_live now makes <b>all</b> SQL tables "live", not just a select few.

	Added modules m_httpd and webcpanel, which provides a web based control panel for users to register, control settings on their nicknames, channels, and memos.
<br/>
	This is still very much a work in progress. If you would like to contribute by improving or creating new templates, or by adding new features to the web panel, feel free to contact us at irc://irc.anope.org/anope.
<br/>
	
MD5 Sum: 9242a522aedc98f74fd09d4e40d12bc6 <a href="https://sourceforge.net/projects/anope/files/anope-devel/Anope%201.9.7/anope-1.9.7-source.tar.gz/download">anope-1.9.7-source.tar.gz</a><br/>
MD5 Sum: bcf37ede4be77f1fd843944e7887ce33 <a href="https://sourceforge.net/projects/anope/files/anope-devel/Anope%201.9.7/anope-1.9.7.exe/download">anope-1.9.7.exe</a>
