---
layout: post
title: Anope 2.1.6 Release
author: Sadie
category: 2024
---

Anope 2.1.6 has been released. This is a development release.

The most notable changes are:

- Added opportunistic upgrading of TLS fingerprints to more secure algorithms on InspIRCd.
- Added support for logging out partially connected users on Plexus.
- Added the account registration time to nickserv/info.
- Changed ns_cert to automatically add a TLS fingerprint to new accounts if available.
- Clarified that a non-deprecated encryption module must be loaded.
- Fixed creating the runtime directory on Windows.
- Fixed mistakenly allowing badpasslimit to be set to a negative value.
- Fixed parsing backup TLS fingerprints on InspIRCd.
- Fixed parsing the flood mode on UnrealIRCd.
- Fixed parsing the history mode on UnrealIRCd.
- Fixed various iterator invalidation issues.
- Partially rewrote the Portuguese translation.
- Removed some incorrect strings from the Turkish translation.
- Renamed the --modulesdir option to --moduledir to match the name of other path options.

The full change log can be found in the `docs` directory or on [GitHub](https://github.com/anope/anope/compare/2.1.5...2.1.6).

Users who want to test out new features are encouraged to upgrade. Before upgrading you may wish to take a backup of your databases and read the [upgrading guide](/upgrading.html). If you encounter any incompatibilities that aren't mentioned on this page then [please open an issue](https://github.com/anope/website/issues/new).

SHA256 Sum: `1fe8805d79b5606c08e82677ab398289940b7ad6a6d63826efdeb4b097a9191c` [anope-2.1.6.tar.gz](https://github.com/anope/anope/archive/refs/tags/2.1.6.tar.gz)
\
SHA256 Sum: `ef84473fe858cf711c1e1bc8153785ec33c137cad0e7c16b21afa4452c4233a0` [anope-2.1.6.exe](https://github.com/anope/anope/releases/download/2.1.7/anope-2.1.6.exe)
