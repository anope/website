---
layout: post
title: Anope 2.0.0-rc4 - Release (updated)
author: DukePyrolator
category: 2014
# date: 2014-03-08T05:12:51+00:00
---

<!--
BEGIN SUMMARY
We are proud to announce the release of Anope 2.0.0-rc4, which is the final release candidate for the final Anope 2.0.0 release.

Once fully released, Anope 2 will replace the current stable branch, 1.8, which will be considered legacy and will no longer be maintained. We will no longer recommend it for use by new networks. However, we intend to continue supporting users currently using 1.8 after the final release for some time, including keeping the download on https://anope.org. Unseating a branch that has been in existance for a decade this March is not an easy task, and we understand it will take some time for users to move over.

While we still classify this release as not production ready, is has a great degree of stability and may very well be the same as the final release. We highly recommend networks wanting to use Anope 2 once it has been officially marked as stable test this release candidate. Bugs can be reported on our bug tracker at <a href="https://bugs.anope.org">https://bugs.anope.org</a>.


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
will not work with Anope 2. However, many of the features of the most popular 1.8 modules have been included in the Anope 2 release, so you may find you no longer need your extra modules. If it is unclear to you whether or not a given feature is in Anope 2, come ask us


<b>Foreign language support:</b>

If foreign languages are not working on your install, see docs/LANGUAGE in the source distribution. Additionally, we only have translators for the Spanish, German, French, Dutch, and Italian languages. The translations for the other languages are out of date, and are built from the old 1.8 language files. However as many of the language strings have changed in the development of 1.9, most of the language strings for the other languages are not translated. If you would like to contribute by translating Anope, we will accept translation updates prior to the final release. Contact us on IRC for more information.


Join our IRC channel at <a href="irc://irc.anope.org/anope">irc://irc.anope.org/anope</a> for questions or comments.




MD5 Sum: 6bebab85c3bc975da965b61c507ffb5b <a href="https://sourceforge.net/projects/anope/files/anope-devel/Anope%202.0.0-rc4/anope-2.0.0-rc4-source.tar.gz/download">anope-2.0.0-rc4-source.tar.gz</a><br/>
MD5 Sum: b9429e6d0777fe6e9d014d9d9ae06abe <a href="https://sourceforge.net/projects/anope/files/anope-devel/Anope%202.0.0-rc4/anope-2.0.0-rc4.exe/download">anope-2.0.0-rc4.exe</a><br/>
END SUMMARY
-->

We are proud to announce the release of Anope 2.0.0-rc4, which is the final release candidate for the final Anope 2.0.0 release.

Once fully released, Anope 2 will replace the current stable branch, 1.8, which will be considered legacy and will no longer be maintained. We will no longer recommend it for use by new networks. However, we intend to continue supporting users currently using 1.8 after the final release for some time, including keeping the download on https://anope.org. Unseating a branch that has been in existance for a decade this March is not an easy task, and we understand it will take some time for users to move over.

While we still classify this release as not production ready, it has a great degree of stability and may very well be the same as the final release. We highly recommend networks wanting to use Anope 2 once it has been officially marked as stable test this release candidate. Bugs can be reported on our bug tracker at <a href="https://bugs.anope.org">https://bugs.anope.org</a>.


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
will not work with Anope 2. However, many of the features of the most popular 1.8 modules have been included in the Anope 2 release, so you may find you no longer need your extra modules. If it is unclear to you whether or not a given feature is in Anope 2, come ask us


<b>Foreign language support:</b>

If foreign languages are not working on your install, see docs/LANGUAGE in the source distribution. Additionally, we only have translators for the Spanish, German, French, Dutch, and Italian languages. The translations for the other languages are out of date, and are built from the old 1.8 language files. However as many of the language strings have changed in the development of 1.9, most of the language strings for the other languages are not translated. If you would like to contribute by translating Anope, we will accept translation updates prior to the final release. Contact us on IRC for more information.


Join our IRC channel at <a href="irc://irc.anope.org/anope">irc://irc.anope.org/anope</a> for questions or comments.




MD5 Sum: 6bebab85c3bc975da965b61c507ffb5b <a href="https://sourceforge.net/projects/anope/files/anope-devel/Anope%202.0.0-rc4/anope-2.0.0-rc4-source.tar.gz/download">anope-2.0.0-rc4-source.tar.gz</a><br/>
MD5 Sum: b9429e6d0777fe6e9d014d9d9ae06abe <a href="https://sourceforge.net/projects/anope/files/anope-devel/Anope%202.0.0-rc4/anope-2.0.0-rc4.exe/download">anope-2.0.0-rc4.exe</a><br/>
