---
layout: post
title: Anope 2.1.2 Release
author: Sadie
category: 2024
---

Anope 2.1.2 has been released, which is the third release on our new development branch.

The notable changes include:

- Added module:tlsv10 to m_ssl_openssl for configuring whether TLSv1.0 is usable (defaults to no).
- Added module:tlsv11 to m_ssl_openssl for configuring whether TLSv1.1 is usable (defaults to yes).
- Added module:tlsv12 to m_ssl_openssl for configuring whether TLSv1.2 is usable (defaults to yes)
- Bumped the minimum OpenSSL version to 1.1.0.
- Bumped the minumum GnuTLS version to 3.0.0.
- Modernized mutex and thread code to use Modern C++.
- Normalised the program exit codes.
- Removed module:sslv3 from m_ssl_openssl.
- Removed the m_ prefix from the names of the chanstats, dns, dnsbl, helpchan, httpd, ldap, ldap_oper, mysql, proxyscan, redis, regex_pcre2, regex_posix, regex_stdlib, regex_tre, rewrite, sasl, sql_log, sql_oper, sqlite, ssl_gnutls, ssl_openssl, xmlrpc, and xmlrpc_main modules.
- Updated the Dutch translation.
- Updated the French translation.

Users who want to test out new features are encouraged to upgrade. Before upgrading you may wish to take a backup of your databases and read the [upgrading guide](/upgrading.html). If you encounter any incompatibilities that aren't mentioned on this page then [please open an issue](https://github.com/anope/website/issues/new).

SHA256 Sum: `16c6cd840c326ea91dc3cab7818034cf30d8604d8d3940c7dca77735a56ab7c3` [anope-2.1.2.tar.gz](https://github.com/anope/anope/archive/refs/tags/2.1.2.tar.gz)
\
SHA256 Sum: `cefd6271d9147a8154eaa7cbae097255d81eb529fffaf737a929773342c70c78` [anope-2.1.2.exe](https://github.com/anope/anope/releases/download/2.1.2/anope-2.1.2.exe)
