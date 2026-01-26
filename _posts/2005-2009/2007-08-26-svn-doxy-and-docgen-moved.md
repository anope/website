---
layout: post
title: SVN, Doxy and Docgen moved
author: GeniusDex
category: 2007
# date: 2007-08-26T04:57:25+00:00
---

<!--
BEGIN SUMMARY
Due to recent server issues, we have moved our SVN repository, WebSVN frontend, Doxygen and Docgen documentation over to a new host. The new links can be found in the menu on the left.
END SUMMARY
-->

Due to recent server issues, we have moved our SVN repository, WebSVN frontend, Doxygen and Docgen documentation over to a new host. They are now hosted at the following locations:</p>

<ul>
<li><span><strong>SVN</strong>: svn://svn.anope.org/anope/</span></li>
<li><span><strong>WebSVN</strong>: <a href="https://dev.anope.org/wsvn/">https://dev.anope.org/wsvn/</a></span></li>
<li><span><strong>Doxygen</strong>: <a href="https://dev.anope.org/doxy/html/">https://dev.anope.org/doxy/html/</a></span></li>
<li><span><strong>Docgen</strong>: <a href="https://dev.anope.org/docgen/">https://dev.anope.org/docgen/</a></span></li>
</ul>

<p>You can move over your local subversion repository to our new host easily. For the SVN command-line client (*nix), enter this in your trunk/ dir to switch the trunk repository to the new location:</p>

<ul><li><span>svn switch --relocate svn://zero.org/repos/anope/trunk svn://svn.anope.org/anope/trunk</span></li></ul>

<p>If you are using TortoiseSVN on Windows, follow these instructions:</p>

<ul>
<li><span>Rightclick on your top svn folder (typically 'trunk'), go to TortoiseSVN, then Relocate...</span></li>
<li><span>At the 'To URL' of the dialog box that popped up, enter <i>svn://svn.anope.org/anope/trunk</i> and click <i>Ok</i></span></li>
</ul>

<p>The links to WebSVN, Doxygen and Docgen can also be found at <a href="https://dev.anope.org/">https://dev.anope.org/</a>. As a bonus you'll get an ASCII-art sketch of our site layout ;)
