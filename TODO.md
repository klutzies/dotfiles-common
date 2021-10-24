GLOBAL:
- Add this repository as a submodule
- Copy dotfiles (gitconfig, gitignore) and other preferences to respective folders via independent scripts in each OS-specific repository
- (some) Microsoft Edge settings
    - Default search engine
    - ...?
- Automate Discord (per OS, but keep prefs here)
  - Disable sticker suggestions
  - Canary
  - Powercord
  - Plugins:
    - Install:
        - Plugin Downloader: https://github.com/LandenStephenss/PowercordPluginDownloader
        - Theme Downloader: https://github.com/ploogins/PowercordThemeDownloader
        - Theme Toggler: https://github.com/redstonekasi/theme-toggler
    - Disable:
        - Hastebin
        - Heygirl
        - LMGTFY
        - Mock
        - Spotify Modal
  - Themes:
    - Dark Discord: https://github.com/snappercord/dark-discord


LINUX:
- We are using Pop!\_OS
- Document Settings (e.g. Dock, "Night Light")
  - Automate this? Should be possible with GNOME command line utilities
- Uninstall Firefox
- Install apps automatically
- Add Microsoft Edge Beta repository
- Add Sublime Text APT repository


macOS:
- adjust keyboard brightness in low light: OFF
- turn keyboard backlight off after ... of inactivity: ON
- MOTD doesn't work (permission denied)
.
- fix battery percentage in menubar in Big Sur
    - also User switcher, Bluetooth, Volume in menubar
.
- automate Sublime Text preferences (plists)
.
- automate Ungoogled Chromium preferences (Chrome profiles?)
.
- automatically copy wallpapers to ~/Pictures/Wallpapers/.
    - apply to System Preferences / Desktop & Screen Saver
        - Change picture: Every 30 minutes
        - Random order
    - maybe download separately instead of bundling with dotfiles
        - wget ZIP from somewhere, then extract to ~/Pictures
        - separate GitHub repo?
.
- disable screensaver; leave power settings as defaults
.
- get rid of all the cruft (namely stuff leftover from winocm fork)
    - organize, organize, organize... (alphabetize defualts-write?)
.
- git clone dotfiles to ~/Projects
    - bootstrap.sh accomplishes half of this
    - can't use git before running dotfiles, can't get dotfiles (with .git) before installing git
    - setup post-install script to be run before reboot (at least after installing Xcode CLT) that connects local repo to remote
.
- upgrade.sh is symlinked... why not symlink it ALL? (./dotfiles/*, etc)
.
- rework menu bar items to account for Big Sur
.
- remove files in ./temporary (fix them accordingly)
.
- research this: https://eclecticlight.co/2017/11/09/customising-it-all-global-defaults-in-macos-sierra-and-high-sierra/
- research this: https://github.com/mathiasbynens/dotfiles
- research this: https://github.com/joeyhoer/starter
.
- rewrite history to be cleaner and more concise... eventually
.
- \[2020/06/09 18:00:36\] - User switcher in menubar
- NO EFFECT
- \[2020/06/09 18:00:36\] - Bluetooth in menubar
- NO EFFECT?
- \[2020/06/09 18:00:36\] - Volume in menubar
- NO EFFECT
- fix menubar prefs as such: https://apple.stackexchange.com/questions/306867/can-defaults-write-command-line-configure-the-menu-bar-on-macos/337179
- enable certain menubar items if we're on a laptop vs. desktop, e.g. check if we're running on MacBook* (sysctl -n hw.model; use bash trickery to check for "MacBook\*")
.
- \[2020/06/09 18:00:\] Setting up defaults for com.apple.Dock from plists/com.apple.Dock.plist.
- BROKEN! save dock setup as image instead
- Set dock according to dock.png
- research macOS dock prefs via `defaults` (i.e. application presence + arrangement) https://hints.macworld.com/article.php?story=20040819170450489
.
- \[2020/06/09 18:00:37\] Setting up defaults for com.apple.finder from plists/com.apple.finder.plist.
- NO EFFECT ON HIGH SIERRA
.
- "Snap to Grid" on Desktop
- Set default folder view options to "Sort by: Kind" (fixed?)
- Create bookmarks according to finder0.png


WINDOWS:
- NOTE: `winget upgrade` does not upgrade programs; it only updates the program database and lists which programs can be upgraded
- Running `winget upgrade --all` "fixes" this; however, it may upgrade Discord, which is not optimal as that will cause Powercord to unplug (a manual replug will be necessary)
- Potential fixes (neither optimal):
    - Exclude Discord from upgrades via built-in `winget` functionality (currently does not exist)
    - Upgrade all programs *except* Discord via regex magic (foreach?)
- Borrow some stuff from here: https://github.com/jayharris/dotfiles-windows
- PowerToys prefs (run as admin on first start)
    - Awake: Off ("keep screen on" doesn't work)
    - Color Picker: On
    - FancyZones: Off
    - File Explorer add-ons: On
    - Image Resizer: Off
    - Keyboard Manager: Off
    - PowerRename: On
    - PowerToys Run: On
    - Shortcut Guide: Off
- Create shortcuts (e.g. start menu sidebar, Explorer sidebar, taskbar items, ~\Desktop\Programs, ~\Desktop\Games, Mouse Jiggler)
- Set Explorer settings (Quick access options, etc.)
- Disable that thing that allows people to connect to you remotely in the same menu Device Manager is in
- Document Settings configuration for Windows 11
