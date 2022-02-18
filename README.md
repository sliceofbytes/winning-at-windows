# winning-at-windows
Windows 11 software and tweaks that *I* find useful. The list is (intentionally) personal and is not meant to be a comprehensive database of all programs of this kind. While the software mentioned below has proven useful to me, not all carbon-based life forms  share the same workflow or tastes. Consider yourself warned.

## "Ricing" (appearance customization)

* [Stardock software](https://www.stardock.com/): Several tools for Windows customization, such as [IconPackager](https://www.stardock.com/products/iconpackager/) (replaces the most common system icons), [WindowFX](https://www.stardock.com/products/windowfx/) (adds effects when opening, closing, minimizing, moving windows), [TouchTasks](https://www.stardock.com/products/touchtasks/) (triggers actions by touching certain screen corners), and [Start11](https://www.stardock.com/products/start11/) (alternative start menu layouts). 

* Fans of alternative start menus will also want to check out [StartAllBack](https://www.startallback.com/) and [Open-Shell](https://github.com/Open-Shell/Open-Shell-Menu).

* [MyDockFinder](https://store.steampowered.com/app/1787090/MyDockFinder/): Mac-like dock and Finder bar. 

* [WinDynamicDesktop](https://github.com/t1m0thyj/WinDynamicDesktop): wallpaper that changes with the time of day, a la MacOS.

* for animated wallpapers, check out [Wallpaper Engine](https://www.wallpaperengine.io/en) or (an open source alternative) [Lively Wallpaper](https://rocksdanister.github.io/lively/)

* [RoundedTB](https://github.com/torchgm/RoundedTB): Add margins and/or rounded corners to the taskbar.

* [OldNewExplorer](https://m.majorgeeks.com/files/details/oldnewexplorer.html): Allows one to return to the good old days when cats were cats, dogs were dogs, and File Explorer was less ornate and cluttered.

* [ModernFlyouts](https://modernflyouts-community.github.io/): Modern-looking pop-up indicators for changing volume, brightness, toggling caps-lock, etc.

* [filetypesman](https://www.nirsoft.net/utils/file_types_manager.html): tool for managing filetype icons and associations.

* [CustomizerGod](https://www.door2windows.com/customizergod/): User-friendly way to replace certain Windows system icons. Was never updated for Windows 11 (or even later builds of Windows 10), so handle with care.

* [Resource Hacker](http://www.angusj.com/resourcehacker/): view and edit resources in EXE, DLL, and related files. Essential tool for changing stubborn icons. To gain permissions to customize icons built in to Windows, you will want to run Resource Hacker with something like [NSudo](https://github.com/M2Team/NSudo). Windows keeps many (but not all) of its icons in **\Windows\SystemResources\shell32.dll.mun** and **\Windows\SystemResources\imageres.dll.mun**.

* [namazso/SecureUxTheme: A secure boot compatible in-memory UxTheme patcher (github.com)](https://github.com/namazso/SecureUxTheme): allows one to apply custom themes without modifying system files, and without rebooting (!) 

* [Rainmeter](https://www.rainmeter.net/): tool for displaying desktop widgets. An endless number of Rainmeter skins are on deviantArt (but beware that many, especially ones that are older, do not play nice with modern high DPI displays). If you use a tablet or frequently change screen resolutions for any other reason, grab [RainRez](https://forum.rainmeter.net/viewtopic.php?f=18&t=10471&hilit=rainrez) as well. 

    * [Droptop](https://github.com/Droptop-Four/Basic-Version/releases/tag/Current-Stable): Rainmeter skin providing a highly customizable menu bar at the top of the screen (think MacOS).
    * [Omnimo](https://omnimo.info/) and [Big Sur](https://www.deviantart.com/fediafedia/art/Big-Sur-1-0-BETA-for-Rainmeter-846882462?comment=1%3A846882462%3A4964685064): two of the most popular (deservedly) skin suites for Rainmeter, by [fediafedia](https://fediafedia.com/).



## System maintenance and optimization

* [SUMo](https://www.kcsoftwares.com/?sumo): Software Update MOnitor. Scans through your installed software to find applications which can be upgraded to a newer version.

* [Process Hacker](https://github.com/processhacker/processhacker): Task Manager replacement. The nightly versions have dark mode support.

* [Chocolatey](https://chocolatey.org/): package manager for Windows, through powershell.

* [Nativefier](https://github.com/nativefier/nativefier): Wrapper to turn webapps into standalone applications.

* [Autoruns for Windows](https://docs.microsoft.com/en-us/sysinternals/downloads/autoruns): comprehensive startup process manager.

* [WizTree](https://diskanalyzer.com/): shows, visually, which files are taking up space on your drive.  Very fast on NTFS-formatted drives. A (paid) alternative with a nicer UI is [FolderSizes](https://www.foldersizes.com/).

* [Bulk Crap Uninstaller](https://www.bcuninstaller.com/): Thorough uninstall tool. Advanced detection capabilities (e.g., knows about programs installed through chocolatey) as well as leftover detection features. A less thorough but much faster-to-start program in the same vein is [geek uninstaller](https://geekuninstaller.com/).

## Usability enhancements

* [ExplorerPatcher](https://github.com/valinet/ExplorerPatcher): restores functionality from Windows 10 that was removed in the "upgrade" to Windows 11 (and does much else besides). I like the clean-looking Alt-Tab replacement that the author built in as well as the taskbar weather widget.

* [Fluent Search](https://www.fluentsearch.net/): Full featured search bar for Windows. The killer feature (for me) is the ability to find a file and drag and drop it from the search window into one of Windows' "open file" dialogue boxes. Huge timesaver.

* [Everything](https://www.voidtools.com/) and [EverythingToolbar](https://github.com/stnkl/EverythingToolbar): Instant search by filename. I have had strange seeming search results with Fluent Search as it comes out of the box; Everything, without trying to be as clever, often gets me directly where I want to go, and it can be configured as the Fluent Search indexing engine. EverythingToolbar seamlessly integrates Everything into the Windows taskbar.

* [Winaero Tweaker](https://winaero.com/winaero-tweaker/): adjust many (!) "secret" Windows settings. For example, you can modify which folders show up under This PC, and you change the Quick Access icon in the navigation pane (though for me this always results in a duplicate navigation pane icon; seems better to avoid WinAeroTweaker for this and just directly edit the registry key `HKEY_CLASSES_ROOT\CLSID\{679f85cb-0220-4080-b29b-5540cc05aab6}\DefaultIcon`).

* [EarTrumpet](https://github.com/File-New-Project/EarTrumpet): Replacement for the Windows system tray audio control widget. Much more functional, e.g., including per-app volume control.

* [BatteryInfoView](https://www.nirsoft.net/utils/battery_information_view.html): Displays information on your battery (e.g., charging status/rate and wear level). An alternative, which can be pinned to the taskbar (on Windows 10, or on Windows 11 if you use something like ExplorerPatcher) is [BatteryBar](https://batterybarpro.com/).

* [BatteryMode](https://github.com/tarcode-apps/BatteryMode): Alternative battery system tray widget. More information than the default widget more customization options too (e.g., bring back the Windows 7 icon).

* [ExtractNow](https://www.extractnow.com/#/home): archive handler. Allows one to unzip/unrar/etc. by double clicking the archive. Quite customizable. 

* [Pantherbar](https://pantherbar-app.com/): Whenever you select text, pops up a menu with possible ``quick actions'' (such as copy, cut, search in Google, run through Google Translate).

* [Snipaste](https://www.snipaste.com/): full-featured and customizable screen snipping tool. Can auto-detect certain portions of the screen that are natural candidates for capture.

* [Seer](http://1218.io): preview a file by pressing the space bar from File Explorer (similar to Quick Look on MacOS). Gets props for having a nice dark mode. 

* [Ditto](https://ditto-cp.sourceforge.io/): good looking clipboard manager for Windows.

* [Incipitor](https://www.dcmembers.com/bgmcoder/download/incipitor/): automates the process of adding shortcuts to the Windows start menu

* [DragDropConfirm](https://github.com/broken-e/DragDropConfirm): shell extension that adds a confirmation dialogue before moving files in File Explorer. Essential for those with touchscreen devices and slippery fingers.

* [TaskbarControl](https://www.thefreewindows.com/3252/hide-completely-the-windows-taskbar-using-a-hotkey-and-unhide-it-with-taskbar-control/): assign a hotkey to hide/unhide the taskbar. Useful for touchscreen devices in combination with Stardock's TouchTasks.

## Icons and other art

* [deviantart](https://www.deviantart.com/): So much to see here! Some of my favorites include (but are not limited to)...
    * anything by [Niivu](https://www.deviantart.com/niivu), especially his Windows themes
    * the  `iconic creations' of [Octaviotti](https://www.deviantart.com/octaviotti)
    * [Mnemo 'n' icons by hechiceroo on DeviantArt](https://www.deviantart.com/hechiceroo/art/Mnemo-n-icons-413224458): gorgeous filetype icons. 

* [500px](https://500px.com): brilliant way to discover photos, many of which make excellent wallpapers.

* [wallhaven](https://wallhaven.cc): large database of wallpapers.

* [IconArchive](https://iconarchive.com/): Remarkably extensive collection of icons. Plug in a keyword and look for something in a style that suits you.

* [macOSicons](https://macosicons.com) has a MacOS-style icon for almost everything.

* those who appreciate the Windows 10/11 icon design language will want to check out the [Fluency collection](https://icons8.com/icons/fluency) at [icons8](https://icons8.com). See also [this repository](https://github.com/icon11-community/Folder11) for folder icons.

* there are an endless number of different styles of Linux icons; I am partial to  elementaryOS. Many icons in that style are collected [here](https://github.com/Macintosh98/elementosh-icons). 

## Hacks

* Open all apps as administrator (registry hack) `REG ADD HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\Policies\System /f /v EnableLUA /t REG_DWORD /d 0/`

* Change taskbar icons of pinned UWP apps. One needs [Win7AppId1.1](https://code.google.com/archive/p/win7appid/downloads). Get the AppID of the desired app by running `get-StartApps | Format-Table | Out-String -width 9999` in PowerShell. Create a custom shortcut  to `explorer.exe shell:appsFolder\YOURAPPID`. Back in Powershell, run `Win7AppId1.1 "YourAppShortcut.lnk" "YOURAPPID"`. Change the icon of the shortcut to whatever you desire, then pin the icon to the taskbar. (Thanks to dpcdpc11 for making me aware of [this method](https://dpcdpc11.com/custom-taskbar-icons-guide/)!)

* Refresh icon cache without restarting Windows. Run (Win+R): `cmd /c taskkill /f /im explorer.exe & del /a %userprofile%\AppData\Local\IconCache.db & start explorer`. You can also create a shortcut with this command as the target. (Taken from [this post](https://superuser.com/a/1300573).)

* Configure Stardock TouchTasks to open Task View. In Windows 10, swiping from the left opened the task view panel. In Windows 11, this action has been remapped to the widgets panel (boo!). You can get close to what we had in Windows 10 with TouchTasks. First, [remove or disable Widgets](https://winaero.com/remove-and-uninstall-widgets-from-windows-11/#:~:text=In%20the%20Local%20Group%20Policy,Click%20Apply%20and%20OK.). Then install [nircmd](https://www.nirsoft.net/utils/nircmd.html) and create a shortcut to `C:\nircmd-x64\nircmd.exe sendkeypress lwin+tab` (replacing the location of nircmd appropriately). Then use TouchTasks to assign the shortcut link to a touchpoint. By default, TouchTasks looks for .exe files, but if you first enter *.lnk in the file dialogue and **then** select your shorcut, it gets properly assigned.

* [mydigitallife forums](https://forums.mydigitallife.net/): These folks are serious about Windows. See, e.g., this very large list of [Windows 11 tweaks, fixes, and modifications](https://forums.mydigitallife.net/threads/windows-11-tweaks-fixes-and-modifications-overview.83744/page-20#post-1687577). Forum registration required.

* [elevenforum](https://www.elevenforum.com/): Another venue for community discussions of Windows customization.  See also [tenforums](https://www.tenforums.com/). The tutorials ([Windows 10](https://www.tenforums.com/tutorials/1977-windows-10-tutorial-index.html), [Windows 11](https://www.tenforums.com/tutorials/1977-windows-10-tutorial-index.html)) are particularly valuable.










