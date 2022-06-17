Maglev Track Set 2.2
===================================
Maglev Track Set 2.2

----------
0 Contents
----------

1   About
2   General information
    2.1  Requirements
    2.2  Installation
    2.3  Parameter settings
    2.4  Usage
3   Known issues
4   Background information
5   Frequently Asked Questions
6   Credits
7   Contact information
    7.1  Bug reports
    7.2  Other problems
    7.3  General enquiries
8   License

-------
1 About
-------

Maglev Track Set v2. This set is the second installment of the Maglev
Track Set, a track set that allows the user to separate their various
maglev trains on different types of tracks for extra realism.
It is also possible to use this set solely to replace the default maglev
tracks. Please refer to 2.4 for instructions on how to do this.

Maglev Track Set 2.2
MD5Hash:  {{GRF_MD5}}
Version:  3
GRF ID:   "EN\02\02"


---------------------
2 General information
---------------------

2.1 Requirements
----------------
- OpenTTD 1.2.0-RC1 or nightly r23971, or higher
- Not compatible with TTDPatch


2.2 Installation
----------------
OpenTTD:
	see http://wiki.openttd.org/NewGRF
	Releases will be available from the ingame Online Content Downloader.
	
2.3 Parameter settings
----------------------
Company colours
	When turned on, the depots will no longer have the real colours, but
	instead use company colours. When turned off the depots will have the
	real colours.
	
Cost Parameters
	With the cost parameters you can set purchase and maintenance costs. You
	can set the costs to the following values:
	1/4x, 1/2x, 1x (default), 2x, 4x

Fences
	With this parameter you can set whether you want fences or not. You can set
	this parameter to the following values:
	None, Only for urban maglevs, Only for high speed maglevs, All railtypes.
	
Override stock maglev track with:
	This parameter is used to override the maglev tracks included by the basegame.
	If no appropriate track is enabled or a trainset does not support this set,
	all maglev trains will/should default to this tracktype.
	Can be set to any of the tracktypes.
	
Tracktypes
	When turned on, the indicated tracktypes will become available. Please make
	sure that the tracktype in the previous parameter is actually enabled.
	
Depot used
	With this parameter you can change the depot used for certain track types
	to the one used by different maglev track types. Visual compatibility is
	not guaranteed.
	
High speed tunnels
	When turned on, high speed tunnels will obtain a custom, brick ground tile
	sprite. Can be used in case a track grf deletes the tunnel ground sprite
	to prevent graphical glitches.
	
  
2.4 Usage
---------
Starting date
    The tracks become available as soon as there are compatible trains.

Replacing base game maglev tracks
	If you just want to replace the base game maglev tracks, set the override
	parameter to the desired maglev tracks and make sure to disable all other
	tracktypes.
	I recommend choosing doing this with the Transrapid or SC-Maglev tracks.
	SC-Maglev for Japanse maglevs, and Transrapid for all others.

Disabling certain tracktypes
	It is often not possible, nor desirable or neccessary to have all tracks
	in the Maglev Track Set. In that case you disable the various tracktypes
	you won't be using. Make sure to set the "override stock maglev" parameter
	to one of the enabled tracktypes. When playing with other tracksets like 
	JapanSet Tracks, not setting the override parameter correctly causes
	problems as OpenTTD can only load 15 tracktypes at once, and the other
	tracksets are already occupying 12 or 13 of those slots, with stock maglev
	and monorail being in the 14th and 15th slot. This should no longer be an
	issue from OpenTTD 1.9.0 onwards.

What trains go on what tracks?
	Transrapid Tracks:
		- Transrapid
		- Future Chinese high speed maglev trains
		- Future Chinese medium-high speed maglev trains: Maglev 3.0
	SC-maglev Tracks:
		- SC-Maglev; the Japanese high speed maglev trains
			- L0 Shinkansen
			- MLX
	SUMA Tracks:
		- Future South Korean high speed maglev trains
	Urban maglev Tracks:
		- HSST and Linimo
		- South Korean low speed maglev trains
		- Chinese low speed maglev trains
		- Future Chinese medium speed maglev trains: Maglev 2.0
		- Future Chinese medium-high speed maglev trains: Maglev 3.0
		- British low speed maglev trains
	M-Bahn Tracks:
		- M-Bahn
		- Future low to medium speed maglev trains developed by Max Bögl
	
For NewGRF developers: How to make your set compatible with this trackset?
	For this trainset we use the labels:
	- TCAS: Transrapid
	- TCAI: SUMA
	- LCAI: SC-Maglev
	- TBAI: Urban Maglev
	- LBAS: M-Bahn
	
	Using a slightly different scheme from the standardised one, as the
	standardised one is not made with Maglevs in mind.
	- - - S : Maglevs that use a synchronous linear motor
	- - - I : Maglevs that use a linear induction motor
	L - - - : Maglevs that have a u-shaped track
	T - - - : Maglevs that have a monorail track
	
	This set also supports the old v1 labels:
	- LCAT: Transrapid
	- LCAE: SC-Maglev
	- LBA3 - LBAT: Urban Maglev
	- LAAT: M-Bahn
	
	There exists a hidden railtype. Trains with this railtype can run on both
	Transrapid, TCAS, and Urban maglev, TBAI tracks:
	- TBAS: Intercity Maglev
	
--------------
3 Known issues
--------------

N/A

------------------------
4 Background information
------------------------

Maglevs > Conventional Rails
Fite me

----------------------------
5 Frequently Asked Questions
----------------------------
What NewGRFs are known to be compatible with this trackset?
	RIMS - Real International Maglev Set https://www.tt-forums.net/viewtopic.php?f=67&t=82345
		- Provides a plethera of new trains. All of which have been marked
		with a symbol as to help you determine what tracktype is appropriate.
	FRIMS - Future Reality Inspired Maglev Set https://www.tt-forums.net/viewtopic.php?f=67&t=85356
		- Meant as an addon to RIMS. Adds maglev trains to last you through the 21st
		century. All of which have been marked with a symbol as to help you determine
		what tracktype is appropriate.
	Modern Maglev Trains (DEPRECATED)
		- This set also provides a lot of new maglev trains. It has been
		superceded by RIMS. The developer insists you use RIMS instead.

---------
6 Credits
---------

Graphics for this set:
- Erato

Code:
- Erato

Makefile system:
- planetmaker (Ingo von Borstel)

---------------------
7 Contact information
---------------------

7.1 Bug reports
---------------
Please report any bugs you find at the
  forum topic: https://www.tt-forums.net/viewtopic.php?f=26&t=76532

Always included a detailed description of the bug, preferrably with
screenshot and savegame. Also state the exact game version you're using, 
as well as the version of this NewGRF.

If you have a savegame that includes NewGRFs not available on OpenTTD's 
Online Content, then please try to reproduce the bug in a new game 
which has all NewGRFs easily accessible.

If you're using a patched version of the game, please try to reproduce
the bug on an official game build. If you can't reproduce the bug, then
don't report it here but in the forum topic of the patch(pack) instead.


7.2 Other problems
------------------
If you have any problems using this NewGRF that are not covered in the 
Frequently Asked Questions above, then you can ask your questions in the
forum topic: https://www.tt-forums.net/viewtopic.php?f=26&t=76532


7.3 General enquiries
---------------------

If you have any queries that cannot be asked in the forum topic, then
contact Erato via Private Message at www.tt-forums.net.


---------
8 License
---------

CC BY-NC 4.0
