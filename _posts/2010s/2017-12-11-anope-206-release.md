---
layout: post
title: Anope 2.0.6 Release
author: Adam
category: 2017
# date: 2017-12-11T18:20:53+00:00
---

Anope 2.0.6 has been released, which contains bug fixes, and several new features.

The notable changes includes:

Log client IP for web clients running commands via webcpanel
<br/>
Fix log file path for the config file could not be opened log message
<br/>
Allow nickserv/group to be used via XMLRPC
<br/>
Fix logsearch without wildcards
<br/>
Support cidr exempts in m_dnsbl
<br/>
Add support for IPv6 dnsbls
<br/>
Add +u and +L channel modes for ircd-hybrid
<br/>
Set +x after hostserv/off on InspIRCd and UnrealIRCd
<br/>
Fix chanserv/mode not being able to set extbans
<br/>
Send CHGIDENT/CHGHOST on SVSLOGIN on InspIRCd
<br/>
Fix escaping replies from commands in webcpanel
<br/>
Enable require_oper for all opers added via operserv/oper
<br/>
Advertise SASL mechanisms to UnrealIRCd servers


All users are recommended to upgrade.

SHA256 Sum: e2a216ab92ceb75b9c8e089d74c4e4e4868b794dd15250d6f8fba3c608f90ccb  <a href="https://github.com/anope/anope/releases/download/2.0.6/anope-2.0.6.exe">anope-2.0.6.exe</a><br/>
SHA256 Sum: 546377755af33f5497a1f5811dfab7d289eaf07b644e4babd1de8d95b9936816  <a href="https://github.com/anope/anope/releases/download/2.0.6/anope-2.0.6-source.tar.gz">anope-2.0.6-source.tar.gz</a><br/>


The news post for the 2.0 branch is reproduced below for those not yet on 2.0. There is no new information here for users already on 2.0.



We are proud to announce that after five years of development our latest stable release, Anope 2.0, is now available for download.

With this release we are deprecating the 1.8 branch and no longer recommend users use it.

<b>Overview of changes from 1.8 to 2.0:</b>

Use an account style system instead of the old NSNickTracking option, which allows you to stay logged in no matter what nick you are on.
<br/>
Fantasy support for all commands.
<br/>
Can assign core pseudo clients (such as ChanServ) to channels.
<br/>
A built in web panel.
<br/>
Persistent channels, which allows services bots to stay in empty channels.
<br/>
Channel passwords replaced with founder level access (QOP, or the FOUNDER access level).
<br/>
OWNER access levels added, defaults to access level 9999.
<br/>
The option to use a flags based channel access system.
<br/>
Ability to authenticate via SSL certificates
<br/>
Autojoin channels on authentication (ns_ajoin)
<br/>
Significantly more advanced logging system, choose what is logged and where it is logged.
<br/>
Support for other optional database backends, such as SQL and Redis.
<br/>
Granular command configuration. Configure which command is on what service, what it's called, and who can use it.
<br/>
Configurable opertypes, which allows defining new services operator levels (Root, Admin, Oper, etc.) and what permissions each has.
<br/>
Ability to authenticate users against external databases, such as by SQL or LDAP.
<br/>
Capability to switch between different encryption methods.
<br/>
DNSBL support.


<b>Installation instructions for Linux/UNIX:</b>

Anope 2 requires CMake to be built. On most systems you can simply install the package from your package manager, eg. sudo apt-get install cmake or sudo yum install cmake.

First, enable any extra modules you want by executing the 'extras' script. Extra modules generally depend on other libraries, such as MySQL, and are not enabled by default due to their dependencies. Then run:

./Config
<br/>
cd build
<br/>
make
<br/>
make install

<b>Upgrading instructions:</b>

1) Install Anope 2 to a separate directory from your old install (such as ~/services2)

2) Copy 1.8's databases to the 'data' directory of your new install.

3) Configure services, the configuration files are located in the 'conf' directory.

   Anope 2 uses a different configuration file format from 1.8, you will have to reconfigure them completely.
<br/>
   Use your old configuration as a reference.

4) While configuring, be sure to load db_old, which loads the old 1.8.x databases, and db_flatfile, which writes out the new Anope 2 database.
<br/>
   Ensure that the hash method in db_old's configuration block is the same encryption method that you are currently using on 1.8.
<br/>
   Load the correct encryption module, which is the same one configured in db_old.

5) Start services. Once you confirm your database has been successfully imported, comment or remove db_old from the configuration file, so that the next time services restart, they will load the newer database.



Third party modules, such as most of the ones found on on the <a href="https://modules.anope.org">Modsite</a>, that are written for 1.7.x or 1.8.x
<br/>
will not work with Anope 2. However, many of the features of the most popular 1.8 modules have been included in the Anope 2 release, so you may find you no longer need your extra modules. If it is unclear to you whether or not a given feature is in Anope 2, come ask us.


Join our IRC channel at <a href="irc://irc.anope.org/anope">irc://irc.anope.org/anope</a> for questions or comments.
