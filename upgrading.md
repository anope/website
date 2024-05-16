---
title: Upgrading from 2.0 to 2.1
layout: simple
---

Upgrading from 2.0 to 2.1 can be done by:

#### General

0. Update any scripts you have that execute `services` to execute `anope` instead.

0. If you are using the `db_sql` or `db_sql_live` modules it is recommended that on 2.0 you load `db_flatfile` and export your database to a file and re-import on 2.1 to update the schema of your database.

#### services.conf

0. Rename `services.conf` to `anope.conf`.

0. Replace `uplink:ipv6` with `uplink:protocol` ([example](https://github.com/anope/anope/blob/2.1.0/data/anope.example.conf#L172-L176)).

0. If you are using the `charybdis` protocol module then migrate to [Solanum](https://github.com/solanum-ircd/solanum) and replace it with the `solanum` module.

0. If you are using the `inspircd3` protocol module then replace it with the `inspircd` module.

0. If you are using the `inspircd12` or `inspircd20` protocol modules then upgrade your IRCd and replace it with the `inspircd` module.

0. If you are using the `unreal4` protocol module then replace it with the `unrealircd` module.

0. If you are using the `unreal` protocol module then upgrade your IRCd and replace it with the `unrealircd` module.

0. Move the `enc_md5`, `enc_none`, `enc_sha1`, and `enc_sha256` modules to be secondary encryption modules and add `enc_argon2`, `enc_bcrypt`, or `enc_sha2` as a new primary encryption module ([example](https://github.com/anope/anope/blob/2.1.4/data/anope.example.conf#L1228-L1345)).

0. Replace the `nickserv/access` privilege in operator accounts with the `nickserv/cert` privilege.

0. Add the `global/queue` and `global/server` privileges to operator accounts with the `global/global` privilege.

0. Update `serverinfo:motd` to be relative to the config directory.

0. Update `serverinfo:pid` to be relative to the data directory.

0. If you are using email then add the `i` flag to the sendmail command ([example](https://github.com/anope/anope/blob/2.1.4/data/anope.example.conf#L953)).

#### botserv.conf

0. Add a description to the `GREET` privilege ([example](https://github.com/anope/anope/blob/2.1.1/data/botserv.example.conf#L326)).

#### chanserv.conf

0. Add a description to the `ACCESS_CHANGE`, `ACCESS_LIST`, `AKICK`, `ASSIGN`, `AUTOHALFOP`, `AUTOOP`, `AUTOOWNER`, `AUTOPROTECT`, `AUTOVOICE`, `BADWORDS`, `BAN`, `FANTASIA`, `FOUNDER`, `GETKEY`, `HALFOP`, `HALFOPME`, `INFO`, `INVITE`, `KICK`, `MEMO`, `MODE`, `NOKICK`, `OP`, `OPME`, `OWNER`, `OWNERME`, `PROTECT`, `PROTECTME`, `SAY`, `SET`, `SIGNKICK`, `TOPIC`, `UNBAN`, `UNBANME`, `VOICE`, and `VOICEME` privileges ([example](https://github.com/anope/anope/blob/2.1.1/data/chanserv.example.conf#L209-L842)).

0. Add the `UNBANME` privilege for `chanserv/unban` ([example](https://github.com/anope/anope/blob/2.1.1/data/chanserv.example.conf#L791-L806)).

0. Remove the `cs_secure` option from `module:defaults` for the `chanserv` module.

#### global.conf

0. Add the `gl_queue` and `gl_server` modules and their commands ([example](https://github.com/anope/anope/blob/2.1.4/data/global.example.conf#L117-L141)).

#### chanstats.conf

0. Remove the `m_` prefix from the `chanstats` module.

#### nickserv.conf

0. Add the `nickserv/set/neverop` and `nickserv/saset/neverop` commands ([example](https://github.com/anope/anope/blob/2.1.0/data/nickserv.example.conf#L581-L582])).

0. Remove the `nickserv/set/secure` and `nickserv/saset/secure` commands.

0. Remove the `ns_access` module and `nickserv/access` command.

0. Remove the `ns_getpass` module and `nickserv/getpass` command.

0. Remove the `ns_status` module and `nickserv/status` command.

0. Remove the `ns_secure` option from `module:defaults` for the `nickserv` module.

0. Rename `nickserv:passlen` to `nickserv:maxpasslen`.

0. Replace `options:strictpasswords` with `nickserv:minpasslen` ([example](https://github.com/anope/anope/blob/2.1.0/data/nickserv.example.conf#L212-L217)).

#### modules.conf

0. If enabled add `module:tlsv10`, `module:tlsv11`, and `module:tlsv12` to the `ssl_openssl` module ([example](https://github.com/anope/anope/blob/2.1.2/data/modules.example.conf#L632-L639)).

0. If enabled remove the `module:sslv3` from the `ssl_openssl` module (now always disabled).

0. If enabled remove the the `m_` prefix from the `dns`, `dnsbl`, `helpchan`, `httpd`, `ldap`, `ldap_oper`, `mysql`, `proxyscan`, `redis`, `regex_pcre2`, `regex_posix`, `regex_stdlib`, `regex_tre`, `rewrite`, `sasl`, `sql_log`, `sql_oper`, `sqlite`, `ssl_gnutls`, `ssl_openssl`, `xmlrpc`, and `xmlrpc_main` modules.

0. If enabled replace the `m_regex_pcre` module with the `regex_pcre2` module.

0. If enabled update `module:cert`, `module:dhparams`, and `module:key` for the `ssl_gnutls` module to be relative to the config directory.

0. If enabled update `module:cert` and `module:key` for the `ssl_openssl` module to be relative to the config directory.

0. If enable replace `module:template` replace for the `webcpanel` module with `module:template_dir` ([example](https://github.com/anope/anope/blob/2.1.4/data/modules.example.conf#L777-L781)).

#### operserv.conf

0. Remove the `os_oline` module and `operserv/oline` command.

#### stats.standalone.conf

0. Remove the `m_` prefix from the `mysql` module.
