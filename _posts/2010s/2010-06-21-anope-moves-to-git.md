---
layout: post
title: Anope moves to Git
author: chaz
category: 2010
# date: 2010-06-21T09:28:53+00:00
---

Since the recent release of Anope 1.9.2 we have taken the decision to migrate our development away from Subversion to Git.

The benefits of this change will outweigh the initial inconvenience of adapting to the new system.

With immediate notice a back up has been taken of the sourceforge subversion repository and will be taken offline.

To access gitweb please click <a href="https://anope.git.sourceforge.net/git/gitweb.cgi?p=anope/anope;a=summary">here</a><br/>

To clone the anope repository you may do the following:

$ git clone git://anope.git.sf.net/gitroot/anope/anope/

The default branch is 1.8 and you can switch to 1.9 by using git checkout -b 1.9 origin/1.9

Further advice is available in the git man page or you may seek support on our web forum.
