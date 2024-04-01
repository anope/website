---
layout: post
title: Anope 2.1.4 Release
author: Sadie
category: 2024
---

Anope 2.1.4 has been released, which is the fifth release on the development branch.

The most notable changes are:

* Added support for importing databases from Atheme.
* Added support for sending client tags on UnrealIRCd.
* Added support for the InspIRCd 1206 (v4) protocol.
* Added the enc_argon2 module to encrypt passwords with Argon2.
* Added the enc_sha2 module to encrypt passwords with HMAC-SHA-2.
* Added the global/queue and global/server command for queueing multi-line messages.
* Added the global/server command for sending messages to an individual server.
* Added the verify-only enc_posix module to validate passwords from Atheme that were encrypted with Argon2.
* Changed nickserv/drop to use confirmation codes to confirm a nickname drop.
* Changed various paths to be relative to the data and config directories.
* Converted the enc_md5, enc_none, enc_old, enc_sha1, and enc_sha256 modules to be verify-only.

The full change log can be found in the `docs` directory or on [GitHub](https://github.com/anope/anope/compare/2.1.3...2.1.4).

Users who want to test out new features are encouraged to upgrade. Before upgrading you may wish to take a backup of your databases and read the [upgrading guide](/upgrading.html). If you encounter any incompatibilities that aren't mentioned on this page then [please open an issue](https://github.com/anope/website/issues/new).

SHA256 Sum: `fb9fba0d331aced342a8bb79a2c898633442d45f6f837f601f48d11a2784e68d` [anope-2.1.4.tar.gz](https://github.com/anope/anope/archive/refs/tags/2.1.4.tar.gz)
\
SHA256 Sum: `bd167747bf094cb623468a53c0c6c69aad06dbc5439199a7453e8b6ead444016` [anope-2.1.4.exe](https://github.com/anope/anope/releases/download/2.1.4/anope-2.1.4.exe)
