FFXIV_ACT_Plugin
================
The ACT Parsing Plugin for Final Fantasy XIV

This project is to track releases and issues for the ACT FFXIV Plugin.  The source code is not currently public.

The DLL file included in this project enables the multi-game parser Advanced Combat Tracker (ACT) to process and display combat information from Final Fantasy XIV patch 6.0. 

DISCLAIMER: Use of this program is at your own risk. Square Enix does not permit the use of any third party tools, even those which do not modify the game.  They have stated in interviews that they did not view parsers as a significant problem unless players use them to harass other players, so the consensus is to not discuss parsers or DPS in-game at all.

I have started a Discord server for discussions regarding this plugin. All are welcome to join, but keep in mind this is for the purpose of developing and improving the plugin, and so may be moderated if discussions go wild.
https://discord.gg/9tHJ7s2P3r

Installation Instructions:

1) Download & install ACT. If you have an existing ACT installation, please remove any other plugins, to ensure there are not any conflicts to start with.  ACT can be downloaded here:<br>
http://advancedcombattracker.com/download.php

2) Launch the ACT Startup Wizard. On the Parsing Plugin tab, click the 'Get Available parsing plugins' button. Choose #73 "FFXIV Parsing Plugin", and click the "Use this plugin" button. Continue the wizard or close it as desired.

3) The FFXIV_ACT_Plugin reads a combination of memory and network data from your local pc.  It has two different ways of accessing the network data:

    a) Default mode - by default, it will use a windows raw socket for the game's network data.  This requires running ACT as a local administrator and adding a firewall rule to permit it to do so.  For Windows Defender it will prompt you to add this rule, but for other firewalls you will need to configure it youtself.
    
    b) Use Npcap kernel driver - If you prefer, you can install Npcap separately from ACT and the FFXIV plugin.  This will allow the plugin to read network data and bypass unique firewall or vpn configurations, and does not require running ACT as an Administrator.  After installing Npcap, the feature can be enabled by going to the ACT Plugins tab, then to the FFXIV ACT Plugin tab, and enabling the "Use Winpcap-compatible library" feature.
 


