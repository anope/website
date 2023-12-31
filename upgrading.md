---
title: Upgrading from 2.0 to 2.1
layout: simple
---

Upgrading from 2.0 to 2.1 can be done by:

#### General

0. Update any scripts you have that execute `services` to execute `anope` instead.

#### services.conf

0. Rename `services.conf` to `anope.conf`.

0. Replace `uplink:ipv6` with `uplink:protocol` ([example](https://github.com/anope/anope/blob/2.1.0/data/anope.example.conf#L172-L176)).

0. If you are using the `inspircd3` protocol module then replace it with the `inspircd` module.

0. If you are using the `inspircd12` or `inspircd20` protocol modules then upgrade your IRCd and replace it with the `inspircd` module.

0. If you are using the `unreal4` protocol module then replace it with the `unrealircd` module.

0. If you are using the `unreal` protocol module then upgrade your IRCd and replace it with the `unrealircd` module.

0. Move the `enc_md5`, `enc_none` and `enc_sha1` modules to be secondary encryption modules and add `enc_bcrypt` or `enc_sha256` as a new primary encryption module ([example](https://github.com/anope/anope/blob/2.1.0/data/anope.example.conf#L1219-L1256)).

#### nickserv.conf

0. Replace `nickserv:strictpasswords` with `nickserv:minpasslen` ([example](https://github.com/anope/anope/blob/2.1.0/data/nickserv.example.conf#L212-L217)).

0. Rename `nickserv:passlen` to `nickserv:maxpasslen`.

0. Remove the `ns_getpass` module and `nickserv/getpass` command.

0. Add the `nickserv/set/neverop` and `nickserv/saset/neverop` commands ([example](https://github.com/anope/anope/blob/2.1.0/data/nickserv.example.conf#L581-L582])).

#### operserv.conf

0. Remove the `os_oline` module and `operserv/oline` command.
