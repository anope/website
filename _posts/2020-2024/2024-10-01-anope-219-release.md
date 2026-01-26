---
layout: post
title: Anope 2.1.9 Release
author: Sadie
category: 2024
---

Anope 2.1.9 has been released. This is a development release.

The most notable changes are:

- Bumped the minimum supported version of UnrealIRCd to 6.
- Fixed granting IRC operator status to services operators.
- Fixed making users an IRC operator on InspIRCd.
- Fixed nonicknameownership on InspIRCd v4.
- Fixed some messages not being translatable.
- Fixed the Argon2 module not having test vectors.
- Increased the default nickname expiry period to one year.

The full change log can be found in the `docs` directory or on [GitHub](https://github.com/anope/anope/compare/2.1.8...2.1.9).

Users who want to test out new features are encouraged to upgrade. Before upgrading you may wish to take a backup of your databases and read the [upgrading guide](/upgrading.html). If you encounter any incompatibilities that aren't mentioned on this page then [please open an issue](https://github.com/anope/website/issues/new).

SHA256 Sum: `1f4f474b42b7360352cc2ceb89f0f70cee40b05c30f1fe12b32d800f2138ff36` [anope-2.1.9.tar.gz](https://github.com/anope/anope/archive/refs/tags/2.1.9.tar.gz)
\
SHA256 Sum: `79a6c69c75ddcb2a9246bf0d72a7f18bda1e9c830d30d6e6a677c08a43ebdb3a` [anope-2.1.9.exe](https://github.com/anope/anope/releases/download/2.1.9/anope-2.1.9.exe)
