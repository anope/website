---
layout: post
title: Anope 2.1.0 Release
author: Sadie
category: 2023
---

Anope 2.1.0 has been released, which is the first release on our new development branch.

The notable changes include:

- Added nickserv:minpasslen for configuring the minimum password length.
- Added support for access list entry descriptions.
- Added support for linking over a UNIX socket.
- Added support for server-initiated logins and logouts on UnrealIRCd.
- Added support for server-initiated logouts on InspIRCd.
- Added support for the ANONYMOUS SASL mechanism.
- Allowed users to opt-out of being added to channel access lists.
- Cleaned up the codebase to use Modern C++17.
- Modernized the build system to use a modern version of CMake.
- Removed nickserv:strictpasswords as it is obsolete now nickserv:minpasslen exists.
- Removed support for using insecure encryption methods as the primary method.
- Removed the Windows-only anopesmtp tool.
- Removed the inspircd12 and inspircd20 modules (use inspircd instead).
- Removed the ns_getpass module (no supported encryption modules).
- Removed the os_oline module (no supported IRCds).
- Removed the two day X-line cap.
- Removed the unreal module (use unrealircd instead)
- Renamed nickserv:passlen to nickserv:maxpasslen.
- Renamed the charybdis module to solanum.
- Renamed the inspircd3 module to inspircd.
- Renamed the unreal4 module to unrealircd.
- Replaced uplink:ipv6 with uplink:protocol.
- Updated all references to IRCServices to refer to Anope instead.

Users who want to test out new features are encouraged to upgrade.

SHA256 Sum: fd46d7cf740deae4557c2e9fd69c791f51a2f00c15659a6d4ea3a0057bfd796b [anope-2.1.0.tar.gz](https://github.com/anope/anope/archive/refs/tags/2.1.0.tar.gz)
\
SHA256 Sum: f91e4b6a385abfe687baa48946c45d49900450a731a8a59d6ad00d88df40575e [anope-2.1.0.exe](https://github.com/anope/anope/releases/download/2.0.14/anope-2.1.0.exe)
