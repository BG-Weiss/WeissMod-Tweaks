Weiss Tweaks
Author: Weiss (cjweiss.com)
Version: 1.0

PREAMBLE
I'm an author. If you like this mod and like reading, consider supporting me by visiting cjweiss.com or buying A Broken Clock Never Boils on Amazon, Kubo, Barnes & Noble, Apple Books, or Smashwords.

OVERVIEW
The purpose of this mod is to fix a couple things that bugged me: namely, the ease of resting and losing both gold and equipped items at the start of Siege of Dragonspear. I prefer full trilogy runs, so I highly recommend these mods with EET. I think COMPONENT 1+4 will work without Enhanced Editions, but I have no intention of supporting/testing it.

There are currently four components.

COMPONENT 1: Pay gold to rest based on elapsed time
The premise of this mod is to add a gold cost to rest rather than hard limiting resting in some way. The amount you have to pay goes up every 20 days of in-game time, the costs capping out at 300 days. If you don't have enough gold, you get a massive fatigue penalty (-6 luck) until proper resting. Additionally, the recommended option adds 4 hours of "beauty sleep" rest. The purpose of this is to increase the "cost" of resting and bring the ratio of time spent resting vs. traveling into closer alignment. These costs are incurred whether sleeping at an inn or in the wild.

The values are intended to force more difficult decisions on when to rest, such as using potions/scrolls on medium-difficulty encounters (where before, I mostly held them for big bosses or simply never used them). The later values rise quickly to push a soft time limit on you. There is a ton of gold to be had in BG1/SoD/BG2, but eventually you'll run out. This mod should push you to keep driving towards the main objectives while allowing plenty (but not infinite) room to side quest.

The default values are below:

DAYS	GOLD COST
0	50
20	500
40	1000
60	1500
80	2000
100	3000
120	4500
140	6000
160	7500
180	9000
200	11000
220	13000
240	15000
260	17500
280	20000
300+	25000

There are 6 options total. You can halve or double the above values, and choose to add (or not) the 4-hour beauty sleep component. For all options, when you travel to Balduran Island for the first time, you'll go back on this table by 1 tier. This is to counteract the days you naturally lose in traveling there.

COMPONENT 2: Keep gold & all equipment at the beginning of Siege of Dragonspear
Heavily recommended if you install Component 1. You will get all your "lost" gold in your starting treasure chest, accompanied by a silly note to roleplay the Ophyillis storyline. Additionally, ALL equipment from your companions (equipped or not) will go to your chest.

COMPONENT 3: Keep gold between Siege of Dragonspear and Baldur's Gate 2

All of your money will be placed behind the locked painting at the start of Irenicus's Dungeon.

NOTE: If skipping SoD, I recommend using EET Tweaks to keep your gear between BG1 and BG2. It may not make sense story wise, but I like the continuity between games. Additionally, the rising gold costs are meant to balance that.

COMPONENT 4: Pay gold to rest based on the number of rests

Similar to COMPONENT 1, this is an alternative method to the rising gold costs of rest. You can use it in place of or in combination with the time-based rest cost. There is also the option to halve or double these costs during install.

# Rests	GOLD COST
0	50
4	500
8	1000
12	1500
16	2000
20	3000
24	4500
28	6000
34	7500
40	9000
44	11000
48	13000
52	15000
56	17500
60	20000
64+	25000

RECOMMENDATIONS/ROLEPLAY

Think of the rising resting costs as mounting repair bills, reagent gathering, antagonistic subterfuge, escalating darkness, or your Bhaalspawn taint needing more lavish feasts to survive.

INSTALLATION:
Run setup-weissmod.exe. Follow the instructions and choose what you want to install. This should be compatible with everything, as long as you are running EET or BG2 only. Based on my understanding of how PartyRested() works, and how this doesn't affect other modded game mechanics, you should install this near the end. The timer for COMPONENT 1 will start ticking when you enter either Candlekeep or Chateau Irenicus (if opting to play only BG2). This means you can install it on an active game, but the timer is not retroactive (i.e. if you are on day 60 when you install and go to Candlekeep, you'll pay the costs for day 0). However...

After starting the timer/counter by going to Candlekeep or Chateau Irenicus (use the console to teleport if needed), you can manually edit what stage of costs you are by using console commands. To do this type...

C:SetGlobal:("weiss_gold_increases","GLOBAL",X)  ---for time based
or
C:SetGlobal:("weiss_rest_count","GLOBAL",X)  ---for rest based

For time-based, X corresponds to the tier on the time-based table minus 1 (so day 60-79 would be 3).
For rest-based, X corresponds to the number of rests.

UNINSTALLATION
It should be safe to uninstall either of these mid-game. However, this is my first mod, so I accept no responsibility for borking your saved game.
