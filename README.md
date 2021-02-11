# Simple Saving

A simple saving mod for gzdoom, attempting to remove savescumming by restricting free saving and instead requiring the use of a resource in order to save.

# Features

* ZScript based
* Complete removal of save-scumming, focusing on resource-based saving instead
* Configuration Menu
* A new button replaces the Save hotkey and prevents saving at-will
    * Saving can be accomplished through the use of a Ankh of Time Manipulation
    * How often these drop, starting amount, and whether they are removed at the end of each level can be configured
* Works for all Doom-Engine games including Doom, Doom 2, Heretic, Hexen and Strife, as well as any other IWADs or PWADs

## Installation and Usage ##

**You will need to set your save hotkey in the Simple Saving options menu before this mod will work properly**

## Building ##

Please note that the repository only contains source code with no transient data (no zscript include files or compiled ACS script)
**Premade release versions are ready to go on the [Releases page](https://github.com/tunbridgep/doom-simplesaving/releases).**

If you wish to build the project yourself, please follow the following steps:

1. Clone or download the repository
2. Compile ACS Scripts. This can be done using [acc](https://zdoom.org/wiki/ACC)
3. Create an include file for all files in the zsc directory. Zscript includes are discussed in detail [here](https://zdoom.org/wiki/ZScript)
4. [Zip the contents of the src directory as a pk3](https://zdoom.org/wiki/Using_ZIPs_as_WAD_replacement), then run in GZDoom by dragging and dropping it onto gzdoom.exe, using the -file parameter or using another method.

Alternatively, a config.json file is provided for use with my [doom-quickbuild](https://github.com/tunbridgep/doom_quickbuild) utility.

## Contributing ##

There are many ways to contribute to the project. The easiest way is by filing a bug report or feature request, however code and documentation contributions are welcome. Documentation of the various features and lighting modes is especially important. All pull requests are welcome, however code should generally follow these rules:

1. ZScript should always be preferred over DECORATE and ACS.
2. Features should be as compatible as possible. Changing or overriding a function or flag on an actor is preferred over simply making a new actor.
3. Almost no thought has been put into multiplayer. This mod has not been tested at all with multiplayer. It is not required for contributions to consider multiplayer, however some consideration would be appreciated. A good example of small considerations is considering whether a console command should exist within the user or server space, and using netevents wherever possible.
4. Consideration should be made for hubs. There is not a significant number of popular hub maps for Doom, however this mod is intended to eventually support Hexen, at which point hub map support will be required. This is usually as simple as checking for e.Reopen when defining/using an event handler.
5. Documentation should be clear. Pull requests and commits should be well documented. Code should be documented where necessary if the intention or logic is not clear. Please follow the existing code style.

For questions or feature suggestions, feel free to create an issue on the issues page, or email me at tunbridge.p+doom@gmail.com

## Credits ##

* Ankh image created by Blue Shadow, taken from [Realm 667](http://realm667.com)

## Other Stuff ##

Checkout my other mods on github

* [Simple Teleporter Effects](https://github.com/tunbridgep/doom-simpleteleportereffects) - add particle effects to any teleporter in any map in a compatible way
* [Simple Saving](https://github.com/tunbridgep/doom-simplesaving) - remove save scumming and tie saving to resource usage.
* [Simple Inventory Items](https://github.com/tunbridgep/doom-inventoryitems) - make most Doom powerups usable from the inventory bar in a compatible way.
* [Simple Completion Rewards](https://github.com/tunbridgep/doom-simplecompletionrewards) - be rewarded for getting 100% completion in a map. Highly configurable.
* [Flashlight Mod](https://github.com/tunbridgep/doom-flashlight) - adds a usable flashlight, the ability to darken the map, a dynamic system for enemy and player stealth, and more.
