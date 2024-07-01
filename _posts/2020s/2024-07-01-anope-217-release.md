---
layout: post
title: Anope 2.1.6 Release
author: Sadie
category: 2024
---

Anope 2.1.7 has been released. This is a development release.

The most notable changes are:

- Added importing of akick reasons, forbid reasons, opers and session exceptions to db_atheme.
- Added support for sending tag messages.
- Added the ability to look up account information of an authenticated user.
- Fixed a crash in ns_cert when an IRC user is not present during a nick registration.
- Fixed a null pointer dereference in the global module.
- Fixed a rare memory leak in os_akill and os_sxline.
- Improved the performance of some code that looks up the primary nick from an account.
- Moved nickserv/set/language and nickserv/saset/language to the ns_set_language module.
- Removed the broken Catalan, Hungarian, and Russian translations.
- Renamed module:expire for the cs_suspend module to suspendexpire.
- Renamed the FANTASIA privilege to FANTASY.
- Reworked the protocol interface for sending messages.
- Updated the Turkish translation.

The full change log can be found in the `docs` directory or on [GitHub](https://github.com/anope/anope/compare/2.1.6...2.1.7).

Users who want to test out new features are encouraged to upgrade. Before upgrading you may wish to take a backup of your databases and read the [upgrading guide](/upgrading.html). If you encounter any incompatibilities that aren't mentioned on this page then [please open an issue](https://github.com/anope/website/issues/new).

SHA256 Sum: `77d0a1ea1da1702d89ec6889fd36966d5250850fdf217a0d93988ab260b82fb7` [anope-2.1.7.tar.gz](https://github.com/anope/anope/archive/refs/tags/2.1.7.tar.gz)
\
SHA256 Sum: `632d3fe325e3cfdfdd3bdbd615e3cfccc6bfb30adc64ebe897dcc90109dc3a28` [anope-2.1.7.exe](https://github.com/anope/anope/releases/download/2.1.7/anope-2.1.7.exe)
