---
layout: post
title: Anope 1.7.18 released
author: GeniusDex
category: 2006
# date: 2006-12-31T17:01:57+00:00
---

<!--
BEGIN SUMMARY
The Anope team starts the new year with the next development release, Anope 1.7.18. Since the previous release, we have been working on the MySQL subsytem to improve stability and security of this code. Next to that, we have added support for encryption modules, finally including support for encrypting passwords with proper MD5 or SHA1.
END SUMMARY
-->

The Anope team starts the new year with the next development release, Anope 1.7.18. Since the previous release, we have been working on the MySQL subsytem to improve stability and security of this code. Next to that, we have added support for encryption modules, finally including support for encrypting passwords with proper MD5 or SHA1.

Next to these two major improvements there are quite a few bugs fixed, including bugs related to module code, internal events, various typo's in the language files, and some IRCd-related issues.

Please note that, due to the big changes, this release might not be as stable as previous development releases. The new MySQL and encryption code have been found stable enough to release to the public, but they might still have undiscovered quirks.

Be sure to check Changes.conf for encryption-related changes to the configuration file. Users of MySQL should also note that the MySQL scheme has been changed in this release and needs to be updated. This can be done using the updates in Changes.mysql.

The source and Windows binaries can be downloaded from <a href="https://sourceforge.net/project/showfiles.php?group_id=94081&package_id=100358&release_id=474910">SourceForge</a>.
