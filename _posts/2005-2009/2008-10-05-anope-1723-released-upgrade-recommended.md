---
layout: post
title: Anope 1.7.23 released -  Upgrade recommended.
author: chaz
category: 2008
# date: 2008-10-05T19:49:04+00:00
---

<!--
BEGIN SUMMARY
** Update **

We have re-released .23 with a revision 'b' as an oversight was made on loading encrypted databases which has now been resolved.

If you previously updated to .23 you needn't update again unless you have problems.

****

Since releasing 1.7.22 just over 2 weeks ago, we've continued to polish the 1.7 branch for the eventual release of 1.8.

We've fixed various issues some shown below:

Buffer overflows with both ChanServ and NickServ (Win32 Crashbug in 1.7.22)

FreeBSD 7 dns_nss.so.1 issue.
<br/>
Expanded behaviour of OperServ Ignore & introduced modular database back end meaning Ignores are saved even after a services restart.
<br/>
Various typographic errors are fixed in help/lang files.
<br/>
Expanded behaviour of OperServ Modlist 
<br/>
Enabled UMODE functionality for InspIRCd 1.1

USERS SHOULD BE AWARE OF BROKEN BACKWARDS DATABASE COMPATIBILITY. TAKE A GOOD BACK UP BEFORE UPGRADING!
END SUMMARY
-->

** Update **

We have re-released .23 with a revision 'b' as an oversight was made on loading encrypted databases which has now been resolved.

If you previously updated to .23 you needn't update again unless you have problems.

****

Since releasing 1.7.22 just over 2 weeks ago, we've continued to polish the 1.7 branch for the eventual release of 1.8.

We've fixed various issues some shown below:

Buffer overflows with both ChanServ and NickServ (Win32 Crashbug in 1.7.22)

FreeBSD 7 dns_nss.so.1 issue.
<br/>
Expanded behaviour of OperServ Ignore & introduced modular database back end meaning Ignores are saved even after a services restart.
<br/>
Various typographic errors are fixed in help/lang files.
<br/>
Expanded behaviour of OperServ Modlist 
<br/>
Enabled UMODE functionality for InspIRCd 1.1

Unfortunately, we encountered some problems with the way in which Chanserv & Nickserv are storing passwords which has led us to make a sad but needed decision to break the long time standing backwards database compatibility with versions prior to this one. - This means that once you have upgraded to 1.7.23 (or any SVN build after revision 1462) you will be unable to go back.

Please make sure you take a back up prior to upgrading just in case you do need to revert!

We cannot stress the importance of this advice, and assure you it was with a heavy heart we broke the compatibility and not a decision we took lightly.

Take a look at our <a href="https://sourceforge.net/project/shownotes.php?group_id=94081&release_id=630915">Changelog</a> for more information

Files

anope-1.7.23b.tar.gz -- Full 1.7.23 source release
<br/>
Anope-1.7.23b.exe -- Windows Installer (No MySQL Support)
<br/>
Anope-1.7.23b-MySQL.exe -- Windows Installer (With MySQL Support)


MD5:

f5c4b500ba3e4ae5021dc8d32bd11d44 *anope-1.7.23b.tar.gz
<br/>
b691368f2e025f3b41301efe7acc9151 *Anope-1.7.23b.exe
<br/>
20e27a95b1864d0dc7e7e28e0f648b00 *Anope-1.7.23b-MySQL.exe
