---
layout: post
title: Anope 2.1.1 Release
author: Sadie
category: 2024
---

Anope 2.1.1 has been released, which is the second release on our new development branch.

The notable changes include:

- Added the UNBANME privilege to allow users to unban themselves.
- Added the m_regex_stdlib module.
- Fixed building on Windows systems without chgrp/chmod.
- Fixed creating sockets in the m_dns, m_httpd, m_proxyscan, and m_redis modules.
- Fixed reading the values of command line arguments.
- Moved core privilege descriptions to the example configs.
- Removed the m_regex_pcre module (use m_regex_pcre2 instead).
- Updated the Italian translation.
- Updated the Polish translation.

Users who want to test out new features are encouraged to upgrade. Before upgrading you may wish to take a backup of your databases and read the [upgrading guide](/upgrading.html). If you encounter any incompatibilities that aren't mentioned on this page then [please open an issue](https://github.com/anope/website/issues/new).

SHA256 Sum: `ba36579322158dc1076e07206aef11564fec60248e59b27eb83897590e67fe6d` [anope-2.1.1.tar.gz](https://github.com/anope/anope/archive/refs/tags/2.1.1.tar.gz)
\
SHA256 Sum: `a36cb766778096b8c4596c39f1fbd09268247a350287ff484a597d7d9113e72b` [anope-2.1.1.exe](https://github.com/anope/anope/releases/download/2.1.1/anope-2.1.1.exe)
