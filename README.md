# Gears of War

## Contents

- [Install Guide > Steam Deck](#install-guide-steam-deck)<br>
  &emsp;[1. Prepare Gears of War DVD](#1-prepare-gears-of-war-dvd)<br>
  &emsp;[2. Install Mozilla Firefox](#2-install-mozilla-firefox)<br>
  &emsp;[3. Install ProtonUp-Qt and GE-Proton10-34](#3-install-protonupqt-and-geproton1034)<br>
  &emsp;[4. Install and configure Lutris](#4-install-and-configure-lutris)<br>
  &emsp;[5. Prepare Gears of War Installer](#5-prepare-gears-of-war-installer)<br>
  &emsp;[6. Run Gears of War Installer](#6-run-gears-of-war-installer)<br>
  &emsp;[7. Launch Gears of War](#7-launch-gears-of-war)
- [Appendix](#appendix)
    - [Mounting an ISO in SteamOS](#mounting-an-iso-in-steamos)
    - [Enable/disable frame limit](#enable-disable-frame-limit)
    - [Skip intro videos](#skip-intro-videos)
- [Credits](#credits)

## Install Guide > Steam Deck

This install guide outlines how to install the PC-DVD version of Gears of War on a factory reset Steam Deck in Desktop Mode. Note that there may be steps that aren't applicable if you have already installed Mozilla Firefox, ProtonUp-Qt, Lutris etc.

### Install Requirements
    Gears of War (PC-DVD)
    External DVD Drive
    Internet Browser
    ProtonUp-Qt
    Lutris

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
3. Configure: `Settings` > `Preferences` > `Runners` > `Wine` > `Configure` > `Runner options` > Wine version: `GE-Proton10-34`
4. Configure: `Settings` > `Preferences` > `Runners` > `Wine` > `Configure` > `System options` > Prefer system libraries: `disabled`

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
    > After the game has been installed, close the Gears of War launch window or confirm the DVD prompt.
4. Optional Frame Limit
> [!NOTE]
> It is recommended that you do NOT disable the frame limit in Gears of War, as highlighted by the [car push sequence](). Note that it can be [toggled manually](https://www.pcgamingwiki.com/wiki/Gears_of_War#High_frame_rate) after installation if you wish to experiment, or the Steam Deck's own frame limiter can be used to cap the frame rate regardless.
5. Installing required DirectX files
> [!NOTE]
> .NET installation will generate xalia.exe prompts - confirm them when they appear.<br>
> .NET installation will automatically open Firefox - minimize Firefox for the remainder of the installation.<br>
5
6. Installing Gears of War Title Updates 1, 2 and 3
> [!NOTE]
> After each update has been installed, close the Gears of War launch window or confirm the DVD prompt.
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
![This application could not be started.](https://github.com/lutris/docs/blob/master/assets/7.png)
3. This prompt appears whenever a prefix that has .NET installed is updated and is [safe to ignore](https://github.com/lutris/docs/blob/master/ProvidingLogs%26SystemInfo.md#wine-rundll32.exe-error), therefore select `No`
4. At the main menu, configure the `Video Settings` as the game will need to be restarted for them to take effect

## Appendix

### Mounting an ISO in SteamOS
1. Open `Dolphin File Manager` > `Settings` > `Configure` > `Configure Dolphin` > `Context Menu` > `Download New Services...`
2. Locate 'Mount Unmount ISO by tazihad' and select `Install`
3. Right-click on an ISO file and mount functionality will now be available: `Mount/Unmount iso image` > `Mount`

### [Enable/disable frame limit](https://www.pcgamingwiki.com/wiki/Gears_of_War#High_frame_rate)

### [Skip intro videos](https://www.pcgamingwiki.com/wiki/Gears_of_War#Skip_intro_videos)

## Credits
Many thanks to the following people for their work that keeps Gears of War playable:
- Launcher Bypass - [njunius](https://github.com/njunius/Gears-of-War-Launcher-Bypass-Update)
- AMD Troika Fix - [adjonesey](https://github.com/CookiePLMonster/SilentPatchME/issues/7#issuecomment-2481542968)
- Gears of War Lutris Scripts - [Lutris](https://lutris.net/games/gears-of-war/) and its contributors
- General Fixes - [PCGamingWiki](https://www.pcgamingwiki.com/wiki/Gears_of_War) and its contributors