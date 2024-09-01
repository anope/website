---
layout: post
title: Anope 2.1.8 Release
author: Sadie
category: 2024
---

Anope 2.1.8 has been released. This is a development release.

The most notable changes are:

- Added account identifiers to the nickserv/info output.
- Added module:preservedisplay to the nickserv module.
- Added support for bool, float, and uint SQL columns.
- Added the ability to automatically determine SQL column types based on the native type.
- Added the nickserv/drop/display oper privilege.
- Added UNIX socket support to mysql module.
- Changed smartjoin to use SendClearBans where available.
- Dropped support for MinGW in favour of native builds.
- Fixed parsing named extbans on InspIRCd.
- Fixed parsing SVSMODE and SVS2MODE from UnrealIRCd.
- Fixed sending global messages to remotely linked servers.
- Removed the services server name from the CTCP version response.

The full change log can be found in the `docs` directory or on [GitHub](https://github.com/anope/anope/compare/2.1.7...2.1.8).

Users who want to test out new features are encouraged to upgrade. Before upgrading you may wish to take a backup of your databases and read the [upgrading guide](/upgrading.html). If you encounter any incompatibilities that aren't mentioned on this page then [please open an issue](https://github.com/anope/website/issues/new).

SHA256 Sum: `8547ce5ef43e010f64a35a1d83fb89567e795589e4661b5f8b0bec7fcd650f52` [anope-2.1.8.tar.gz](https://github.com/anope/anope/archive/refs/tags/2.1.8.tar.gz)
\
SHA256 Sum: `b349f3b1b9ab982ab7b54a663c94c8d9bc95e6d73fe077a306f2874b31ae2f42` [anope-2.1.8.exe](https://github.com/anope/anope/releases/download/2.1.8/anope-2.1.8.exe)
