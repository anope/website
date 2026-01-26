---
layout: post
title: Anope 2.1.3 Release
author: Sadie
category: 2024
---

Anope 2.1.3 has been released, which is the fourth release on the development branch.

The notable changes include:

* Added alternate command suggestions when a user runs an invalid command.
* Added support for multiple SSL fingerprints in oper:certfp.
* Added support for the IRCv3 +draft/channel-context tag.
* Added support for the IRCv3 +draft/reply tag.
* Added the chanserv/cert oper privilege for modifying other user's certificate lists.
* Allow using more than one fingerprint in an oper block.
* Changed chanserv/drop to use confirmation codes to confirm a channel drop.
* Changed networkinfo:chanlen to default to 32 if not set.
* Changed networkinfo:hostlen to default to 64 if not set.
* Changed networkinfo:modelistsize to default to 100 if not set.
* Changed networkinfo:nicklen to default to 31 if not set.
* Changed networkinfo:userlen to default to 10 if not set.
* Cleaned up more of the codebase to use Modern C++17.
* Enabled using more field limits sent by the IRC server instead of requiring the user to configure them.
* Fixed NickServ lying about the minimum password length.
* Fixed a crash when sending emails.
* Fixed bs_kick not using the correct kick message for automatic kicks.
* Increased the default maximum password length to 50 characters.
* Increased the default minimum password length to 10 characters.
* Increased the security of randomly generated confirmation codes.
* Removed the cs_secure option in module:defaults from the chanserv module (now always enabled).
* Removed the nickserv/saset/secure command.
* Removed the nickserv/saset/secure oper privilege.
* Removed the nickserv/set/secure command.
* Removed the nickserv/status command.
* Removed the ns_access module and associated cs_secure and ns_secure options.
* Removed the ns_secure option in module:defaults from the nickserv module (now always enabled).
* Reworked how messages are sent in protocol modules to allow sending message tags.

Users who want to test out new features are encouraged to upgrade. Before upgrading you may wish to take a backup of your databases and read the [upgrading guide](/upgrading.html). If you encounter any incompatibilities that aren't mentioned on this page then [please open an issue](https://github.com/anope/website/issues/new).

SHA256 Sum: `be48cc22faef983dedc2d904feb34a77573c36db6ceed829a970cfefa6d024c7` [anope-2.1.3.tar.gz](https://github.com/anope/anope/archive/refs/tags/2.1.3.tar.gz)
\
SHA256 Sum: `162127419a89b0a0e790215b192e71a997b64af77c76b26fb2b67cbc977ec80a` [anope-2.1.3.exe](https://github.com/anope/anope/releases/download/2.1.3/anope-2.1.3.exe)
