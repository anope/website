---
layout: post
title: Anope 1.7.17 released - URGED TO UPGRADE
author: GeniusDex
category: 2006
# date: 2006-10-17T13:10:47+00:00
---

<!--
BEGIN SUMMARY
The Anope team would like to announce the immediate availability of Anope 1.7.17. This version is the latest in the development series of Anope and fixes a possible remote exploit when used with MySQL. This possible exploit is present in nearly ALL 1.7-versions of Anope and we therefore urge anyone running Anope 1.7.1 or newer to upgrade to 1.7.17 as soon as possible.
END SUMMARY
-->

The Anope team would like to announce the immediate availability of Anope 1.7.17. This version is the latest in the development series of Anope and fixes a possible remote exploit when used with MySQL. This possible exploit is present in nearly ALL 1.7-versions of Anope and we therefore urge anyone running Anope 1.7.1 or newer to upgrade to 1.7.17 as soon as possible.

This release also includes a number of other MySQL related fixes, which should patch the current MySQL code sufficiently to be used safely, as well as minor fixes to compiling and anoperc.

PLEASE NOTE: The MySQL schema has been changed in this release. Please consult the Changes.mysql file for MySQL queries to update your tables for use with Anope 1.7.17; Anope won't function correctly when using MySQL without these adjustments!

Anope's Quality Assurance team has reviewed various code sections related to the issues fixed in Anope 1.7.17. On their advice the proposed release of 1.8.0 will be postponed to allow the development team to clean up various sections of code. During this time, some additional features postponed during the feature freeze will be added to the development branch for inclusion in the stable 1.8 series.

The new release can, as always, be downloaded from <a href="https://sourceforge.net/project/showfiles.php?group_id=94081&package_id=100358&release_id=456447">SourceForge</a>.
