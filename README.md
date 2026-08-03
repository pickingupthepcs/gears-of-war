# Gears of War

## Install Guide - Steam Deck

This install guide outlines how to install the PC-DVD version of Gears of War on a factory reset Steam Deck in Desktop Mode. Note that there may be steps that aren't applicable if you have already installed Mozilla Firefox, ProtonUp-Qt, Lutris etc.

### Install Requirements
- Gears of War (PC-DVD)
- External DVD Drive
- Internet Browser
- ProtonUp-Qt
- Lutris

### 1. Prepare Gears of War DVD
Gears of War can be installed using any of the following four methods:<br>
`Method 1`: Mount the Gears of War DVD and install directly from the DVD<br>
`Method 2`: Mount the Gears of War DVD and copy the contents to a dedicated folder (slow)<br>
`Method 3`: [Mount the Gears of War ISO](#mounting-an-iso-in-steamos) and install directly from the ISO<br>
`Method 4`: [Mount the Gears of War ISO](#mounting-an-iso-in-steamos) and copy the contents to a dedicated folder

### 2. Install Mozilla Firefox
1. Select the `Firefox` icon in the taskbar, or open `Discover` and search 'Firefox'
2. Install and launch `Firefox`
3. Upon completing the introduction process, close Firefox

### 3. Install ProtonUp-Qt and GE-Proton10-34
1. Open `Discover` and search 'ProtonUp-Qt'
2. Install and launch `ProtonUp-Qt`
3. Select `Add version`, `GE-Proton10-34` and `Install` to start downloading GE-Proton10-34
4. Upon completing the download, close ProtonUp-Qt

### 4. Install and configure Lutris
1. Open `Discover` and search 'Lutris'
2. Install and launch `Lutris`
3. Configure Wine: `Settings` > `Preferences` > `Runners` > `Wine` > `Configure`
    1. `Runner options` > Wine version: `GE-Proton10-34`
    2. `System options` > Prefer system libraries: `disabled`

### 5. Prepare Gears of War Installer
1. Download [gears-deck-dvd.yaml](https://github.com/pickingupthepcs/gears-of-war/blob/main/gears-deck-dvd.yaml)
2. Launch `Lutris` if closed
3. Select `Add Game [+]`
4. Select `Install from a local install script`
5. Locate `gears-deck-dvd.yaml`, then `Install`
7. Select Steam Deck Installer, then `Install`
6. Select your installation directory, then `Continue`
7. Select whether to download or locally source additional files, then `Install`

### 6. Run Gears of War Installer
1. Installing required System DLLs
2. Locate Gears of War DVD
    1. Select `Browse...`
    2. Locate [Gears of War DVD directory](#1-prepare-gears-of-war-dvd)
3. Installing Gears of War
    1. Select `Install` in the Gears of War setup window
    2. Proceed through the game installation
> [!NOTE]
> **🚩 After the game has been installed, close the launch window or confirm the DVD prompt.**
4. Optional Frame Limit
> [!NOTE]
> **🚩 It is recommended that you do NOT disable the frame limit in Gears of War.**<br>
> **🚩 High frame rate issues are highlighted in the [car push sequence]().**<br>
> **🚩 The frame limit can be [toggled manually](https://www.pcgamingwiki.com/wiki/Gears_of_War#High_frame_rate) if you wish to experiment.**<br>
> **🚩 The Steam Deck's own frame limiter can also be used to cap the frame rate regardless.**
5. Installing required DirectX files
> [!NOTE]
> **🚩 .NET installation will generate xalia.exe prompts - confirm them when they appear.**<br>
> **🚩 .NET installation will open Firefox - minimize it for the remainder of the installation.**<br>
6. Installing Gears of War Title Updates 1, 2 and 3
> [!NOTE]
> **🚩 After each update has been installed, close the launch window or confirm the DVD prompt.**
7. Completion
    1. Select `Close` in the installer window
    2. Return to the `Games` page in Lutris
    3. Right-click on Gears of War and select `Create application menu shortcut`
    4. Right-click on Gears of War and select `Create Steam Big-Picture shortcut`
    5. Close Lutris
    6. Return to Gaming Mode

### 7. Launch Gears of War
1. In Gaming Mode, go to `Library` > `NON-STEAM` > `Gears of War` and select `Play`
2. On first launch the following prompt will be displayed
   
<p align="center">
  <img src="https://github.com/lutris/docs/blob/master/assets/7.png">
</p>

3. This prompt appears whenever a prefix that has .NET installed is updated, and is [safe to ignore](https://github.com/lutris/docs/blob/master/ProvidingLogs%26SystemInfo.md#wine-rundll32.exe-error)
4. Select `No`

## Appendix

### Mounting an ISO in SteamOS
1. Open `Dolphin File Manager`
2. Select `Settings` > `Configure` > `Configure Dolphin` > `Context Menu` > `Download New Services...`
3. Locate 'Mount Unmount ISO by tazihad' and select `Install`
4. Right-click on an ISO file and mount functionality will now be available: `Mount/Unmount iso image` > `Mount`

### [Enable/disable frame limit](https://www.pcgamingwiki.com/wiki/Gears_of_War#High_frame_rate)

### [Skip intro videos](https://www.pcgamingwiki.com/wiki/Gears_of_War#Skip_intro_videos)

## Credits
Many thanks to the following people for their work that keeps Gears of War playable:
- Launcher Bypass - [njunius](https://github.com/njunius/Gears-of-War-Launcher-Bypass-Update)
- AMD Troika Fix - [adjonesey](https://github.com/CookiePLMonster/SilentPatchME/issues/7#issuecomment-2481542968)
- Gears of War Lutris Scripts - [Lutris](https://lutris.net/games/gears-of-war/) and its contributors
- General Fixes - [PCGamingWiki](https://www.pcgamingwiki.com/wiki/Gears_of_War) and its contributors
