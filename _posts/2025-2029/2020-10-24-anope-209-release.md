---
layout: post
title: Anope 2.0.9 Release
author: Sadie
category: 2020
# date: 2020-10-24T23:27:07+00:00
---

Anope 2.0.9 has been released, which contains a fix for a regression in 2.0.8 regarding account identifiers and MySQL database serialisation.

The notable changes includes:

Fix a regression from 2.0.8 that prevented serialising to MySQL.
<br/>
Send account identifiers to InspIRCd on SASL logins too
<br/>
Fix a query bug in irc2sql.

If you have already upgraded to 2.0.8 and are using db_sql or db_sql_live you can avoid data loss by loading the db_flatfile backend, rehashing, and then force saving to disk using <code>/msg OperServ UPDATE</code>. Once you have upgraded to 2.0.9 you can use the import feature of db_sql to reimport your data to the SQL database. See <a href="https://wiki.anope.org/index.php/2.0/Modules/m_sql">the wiki</a> for more details.

All users are recommended to upgrade.

SHA256 Sum: d098ac3cd273c7a243fb1e32ce7aa702f09a6ca3d821a4544f72ef4d1f29ec36 <a href="https://github.com/anope/anope/archive/2.0.9.tar.gz">anope-2.0.9.tar.gz</a><br/>
SHA256 Sum: 512208431e5a9d5714b2a5106916e90b5d1854ce394e0faff21d8c15336e097b  <a href="https://github.com/anope/anope/releases/download/2.0.9/anope-2.0.9.exe">anope-2.0.9.exe</a>
