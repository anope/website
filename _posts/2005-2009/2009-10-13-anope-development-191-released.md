---
layout: post
title: Anope Development 1.9.1 Released
author: chaz
category: 2009
# date: 2009-10-13T19:25:39+00:00
---

Almost 6 months to the day since we released a patched build of 1.9.0 (aptly named 1.9.0-p1) and as time has gone on more and more has been achieved from what is proving to be a fast paced development cycle. (I know many people will be pleased to hear that).

Not only have we completed the goals we set out on our road map <a href="https://anope.svn.sf.net/viewvc/anope/trunk/TODO">here</a> we have put in some extra bits along the way in what is in the words of one of our team members Adam's own words what makes this release "BIG".

Some highlighted changes we want to mention:
<br/>
============================================

* Account functionality has been introduced (and will continue to evolve) so you don't have to group every single nickname you use if it's only a temporary fixture such as chaz|birthday, chaz|brbsuicide, etc. A knock on from this means you will need to /NS LOGOUT before you can group nicks to your account but we're looking at whether we can automate this functionality for later.

* Fantasy Commands - We know how much people love our very own Viper's bs_fantasy_ext module and how troubled you all were when it wasn't available for 1.9.x well now you don't even need it, the majority and some more functionality have been put into Chanserv directly, give it a go, tell us if we've missed anything!

* Opertypes - We've listened and responded to people wanting to provide granular access to commands on their own terms, not being stuck to fixed roles as previously so starting with 1.9.1 you will be able to declare your own oper types, assign them specific or blanket permissions and even allow non-opers to use commands on all pseudo clients EXCEPT Operserv (OSOpersOnly enabled by default) which many people wanted to do by allowing help operators perform some tasks that previously only a services oper (and in turn an irc operator) could only do. 

* Improved InspIRCd 1.2 Support - We've worked very hard to bring good support for this newly released as stable version of InspIRCd. A big thanks to those guys for being approachable and helping us innovate and build improved platform support together. I can predict a bright future continuing to work with these guys to make it happen.

& many many more.

MD5 Checksums:

e1bda0c09c9b926ee50b708b3c3eaa7b  anope-1.9.1-source.tar.gz
<br/>
38dca4ca861c4b9fa2d1b5519bd49cbe  anope-1.9.1.exe


<a href="https://sourceforge.net/projects/anope/files/">Sourceforge Download Links</a><br/>
<a href="https://www.anope.org/downloads/Anope%201.9.1/">Anope Mirrored Download Links</a><br/>


What can you expect from this release?
<br/>
======================================

Well, first of all, don't expect it to be absolutely rock solid stable as it's only the second (well third) release of a completely rehashed and rejigged/redeveloped code base! Similarly though you can have confidence that it's been well tested and abused by several of us on our own live networks so we do have a great deal of confidence in it!

At the moment, we do not know of any issues that aren't taken care of, but as always we welcome your support in helping us nip bugs in the bud nice and quickly by signing up at our simplified sign on portal https://login.anope.org and posting a bug over at https://bugs.anope.org

Providing accurate and detailed information will help us help you quicker.


What do we need from you?
<br/>
=========================

We need you folks to pick this version up, get it compiled on your testnet (or live net if you really want to work with the most bleeding edge and rapid paced development) and help us put it through its paces, do the things your users do day in day out, help us find any oddities, help us continue to pushing the offering further and further whilst building confidence and getting involved yourselves. We don't bite. Well, we do sometimes but that's only if you don't read the rules or act like an idiot.


Network Testing Group
<br/>
=====================

We want people who are genuinely interested in the future of Anope to get involved and help us by testing, and making suggestions to the future. We can't do this without you folks and if you don't get involved you can't complain later about not liking something!

Interested? Email me, chaz@anope.org and we'll have a chat.

Even if you're interested in doing something completely different, do drop me an email, there's always stuff to be done and we're always open to new ideas!


Special mentions
<br/>
================

I'd like to personally mention some thanks as it's not often we receive praise from genuinely happy users, normally it's a question of why raw doesn't work or why services won't link to my network. 

The team have all worked very hard in bringing this release to you, but more than that, community involvement is increasing and I'm really really pleased with this and hope that it continues this way.

You are all very welcome to join us on irc.anope.org in #anope to help or get help, #anope-devel if you want to get stuck in with the development of modules or the core itself, and finally #anope-social if you want to let off some steam and chill out in a relaxed (safe from my ban hammer) environment.

Finally, a very humbled thank you to the two people who have donated to the project recently (you guys rock and you know it), and also a massive thank you to our very own Jens (Duke Pyrolator) for donating the use of a dedicated server until next Summer! This has recently taken on the load of our web platform where we're getting hundreds of thousands of hits each month. Thanks again Duke.
