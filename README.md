# Simple Saving

A simple saving mod for doom, attempting to remove savescumming by restricting free saving and instead requiring the use of a resource in order to save.

# Features

* ZScript based
* Complete removal of save-scumming, focusing on resource-based saving instead
* Configuration Menu
* A new button replaces the Save hotkey and prevents saving at-will
    * Saving can be accomplished through the use of a Ankh of Time Manipulation
    * How often these drop, starting amount, and whether they are removed at the end of each level can be configured
* Works for all Doom-Engine games including Doom, Doom 2, Heretic, Hexen and Strife, as well as any other IWADs or PWADs

# Installation

**Release versions are ready to go from the [releases](releases) page. Simply download a release version and drag it onto gzdoom.exe to start playing**

## Building

Please note that the repository only contains source code with no transient data (no zscript include files or compiled ACS script)

If you wish to build the project yourself, please follow the following steps:

1. Clone or download the repository
1. Compile ACS Scripts. This can be done using [acc](https://zdoom.org/wiki/ACC)
2. Create an include file for all files in the zsc directory. Zscript includes are discussed in detail [here](https://zdoom.org/wiki/ZScript)
3. [Zip the contents of the src directory as a pk3](https://zdoom.org/wiki/Using_ZIPs_as_WAD_replacement), then run in GZDoom by dragging and dropping it onto gzdoom.exe, using the -file parameter or using another method.

Alternatively, a config.json file is provided for use with my [doom-quickbuild](https://github.com/tunbridgep/doom_quickbuild) utility.

# Credits

* Ankh image created by Blue Shadow, taken from [Realm 667](http://realm667.com)
