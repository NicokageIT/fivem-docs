---
title: Client FAQ
weight: 810
---

Will FiveM run on Xbox or Playstation?
-------------------------------------

No. FiveM is developed exclusively for the PC version of GTA V. There are no plans to support consoles.

Will FiveM run on Linux?
------------------------

The FiveM client cannot run on Linux due to [no support](https://github.com/doitsujin/dxvk/issues/899) for shared resources in DXVK. You can run a FiveM server on Linux.

Where is FiveM installed?
-------------------------

That depends on how you installed it in the first place.

- Did you run FiveM.exe in an empty folder? Then that's where FiveM is installed.
- Otherwise, FiveM installs in `%localappdata%`:
    - Press `WinKey+R` on your keyboard
    - Type `%localappdata%/FiveM` in the dialog that opens
    - Hit Enter

More about installing FiveM [here][installing-fivem].

Will I get banned from GTA:Online for playing FiveM?
---------------------------------------

Nope! [As mentioned on fivem.net](https://fivem.net/#no-bans), FiveM does not interact with the Rockstar Online Services other than to validate your game copy the first time you launch it. This validation emulates the game's interaction, and can not be detected by Rockstar. It also doesn't modify your game files at all, even when downloading server assets, so you don't have to do anything to move between FiveM or GTA:O.

**How does the CitizenFX.ini file work?**
---------------------------------------
First of all, it is an .ini file, an initialization file, which means it is a relatively important file since its task is to ensure that the settings within it are correctly triggered when FiveM starts.

These are the various conventional settings that can be set:
[Game] -- game section
IVPath=E:\SteamLibrary\steamapps\common\Grand Theft Auto V      -- e.g. of a gta5 files location
SavedBuildNumber=3095
UpdateChannel=production

[Addons] -- example of an addon, addons section
ReShade5=ID

**functionality**
- IVPath is the string where the file path of GTA5 is entered as a value, so FiveM at startup will refer to that file path for GTA5.exe. Certainly, if the game is not original or there is nothing in that path, it will give an error.
- SavedBuildNumber is the string that refers to which version of the DLC is being used from the last server we accessed.
- UpdateChannel is the string that refers to which type of update reception channel we are using, that is, we are using FiveM in
   - production (release), the stable version recommended for general use;
   - beta, the version in advanced testing, with new features but potentially unstable;
   - canary (latest), the most updated and least tested version, with potential bugs and instability.

I'm running into issues, what can I do? 
---------------------------------------

It's never fun to run into problems. Read the [client issues manual][client-issues] for help.

[installing-fivem]: /docs/client-manual/installing-fivem
[client-issues]: /docs/support/client-issues
