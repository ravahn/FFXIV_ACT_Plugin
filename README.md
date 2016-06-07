FFXIV_ACT_Plugin
================
The ACT Parsing Plugin for Final Fantasy XIV

This project is to track releases and issues for the ACT FFXIV Plugin:<br>
http://www.eq2flames.com/plugin-discussion/98088-ffxiv-arr-plugin.html<br>
The source code is not currently public.

The DLL file included in this project  enables the multi-game parser Advanced Combat Tracker (ACT) to process and display combat information from Final Fantasy XIV patch 3.3. 

DISCLAIMER: Use of this program is at your own risk. Square Enix does not permit the use of any third party tools, even those which do not modify the game.  They have stated in interviews that they did not view parsers as a significant problem unless players use them to harass other players, so the consensus is to not discuss parsers or DPS in-game at all.

Installation Instructions:

1) Download & install ACT. If you have an existing ACT installation, please remove any other plugins, to ensure there are not any conflicts to start with.  ACT can be downloaded here:<br>
http://advancedcombattracker.com/download.php

2) Launch the ACT Startup Wizard. On the Parsing Plugin tab, click the 'Get Available parsing plugins' button. Choose #66 "FFXIV Parsing Plugin", and click the "Use this plugin" button. Continue the wizard or close it as desired.

3) Make a decision to either:
* Parse FFXIV data by scanning network data sent to FFXIV.  This will improve the overall parse quality, because network data is communicated reliably to the plugin, and includes some data which is not available in memory.  If you choose this:
    a) You must run ACT as an Administrator.
    b) You must configure your firewall software to allow ACT to communicate through it.  Reddit user Xepher01 contributed some instructions for Windows 7  <a href="http://imgur.com/a/QU86T">here</a>, and EQ2Flames user Aristar added instructions for windows 8 & 10  <a href="http://imgur.com/a/HiGKr">here</a>.
* If you prefer to not use this data, you can instead parse from game memory.  To do this, you must check the "Disable Parsing from Network Data" checkbox on the FFXIV Settings tab inside ACT.  
 
However, keep in mind that there are known problems with memory-only parsing that will cause some combat information to be lost.  Network mode is more accurate, and should always be used when comparing parses between players.

More information to come.



