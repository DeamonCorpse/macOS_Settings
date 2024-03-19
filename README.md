# macOS SETTINGS
## SYSTEM PREFERENCES
### CONTROL CENTER
- Wifi: Show in Menu Bar
- Bluetooth: Don't Show in Menu Bar
- Air Drop: Don't Show in Menu Bar
- Focus: Show when Active
- Stage Manager: Don't Show in Menu Bar
- Screen Mirroring: Show when Active
- Display: Show when Active
- Sound: Show when Active
- Now Playing: Show when Active
- Battery: Show in Control Center
- Fast User Switching: Show in Control Center
- Keyboard Brightness: Show in Control Center
- Menu Bar Only:
  - Spotlight: Don't Show in Menu Bar
  - Siri: Don't Show in Menu Bar
  - Time Machine: Show in Menu Bar
  - VPN: Show in Menu Bar
- Automaticallt Show & Hide the Menu Bar: In Full Screen Only
- Recent Docs, Apps & Servers: 5
<br>

### DESKTOP & DOCK
- Position on Screen: Bottom
- Minimize Windows Using: Scale Effect
- Double-Click a Window's Title Bar to: Zoom
- Minimize Application Window into Icon: On
- Automatically Hide & SHow the Dock: On
- Animate Opening Applications: On
- Show Indicators for Open Applications: On
- Desktop & Stage Manager:
  - Show Items:
    - On Desktop: On
  - Click wallpaper to reveal desktop: Only in Stage Manager
  - Widgets:
    - Show Widgets On Desktop -> On
    - Widget Style: Full Color
    - Use iPhone Widgets: On
  - Default Web Browsere: Arc
  - Windows:
    - Prefer Tabs when Opening Documents: Always
    - Ask to Keep Changes when CLosing Documents: On
    - Close Windows when Quitting an Application: On
  - Mission Control:
    - Group Windows by Application: On
  - Hot Corners:
    - Top Left: ⌥ Start Screen Saver
    - Bottom Left: ⌥ Put Display to Sleep
    - Top Right: ⌥ Notification Center
    - Bottom Right: ⌥ Quick Note
<br>

### SCREEN SAVER
- [Matrix](https://github.com/monroewilliams/MatrixDownload/)
- Show on all Spaces: On
<br>

### GAME CENTER
- Disabled
<br>

## macOS APPLICATIONS
### FINDER SETTINGS
- General:
  - Show these on the Desktop: External Disks
  - New Finder Windows Show: Downloads
  - Open Folders in Tabs Instead of New Windows: Checked
- Tags: Evedrything Unchecked
- Sidebar:
  - Checked: Applications, Downloads, Home iCloud Drive, Desktop, Hard Disks, External Disks, Cloud Storage, Bonjour Computers, Connected Servers
- Advanced:
  - Show all filename extensions: Checked
  - Show warning before changing an extension: Checked
  - Remove Items from the Trash After 30 Days: Checked
  - When Performing a Search: Search the Current Folder
- View:
  * As List
  * Sort By: Name
  * Show Toolbar
  * SHow Path Bar
  * Show Status Bar
<br>

## 3RD PARTY APPLICATIONS
*Unless otherwise specified, all 3rd party applications are installed using `brew`*

### HOMEBREW
[Homebrew](https://brew.sh/) is dubbed as the missing macOS package manager and allows us to install tools and apps from the command line.
- Installed using the command on the brew homepage. *It will also install Apple's 'Command Line Tools for Xcode' as a dependency.*
- Download the `txt` files inside the `brew` folder of this repo
- Run the following commands to install all casks (applications) and formulae (cli tools):

```sh
xargs brew install < brew_casks.txt
xargs brew install < brew_formulae.txt
```
<br>

### RAYCAST - Replacing Spotlight
*Raycast is installed as a cask by `homebrew`*<br>
`Spotlight` is replaced by [RayCast](https://www.raycast.com/).
- Disable `Spotlight` shortcut in Settings/Keyboard/Keyboard Shortcuts/Spotlight

#### EXTENSIONS
- [Apple Reminders](https://www.raycast.com/raycast/apple-reminders)
- [Arc](https://www.raycast.com/the-browser-company/arc)
- [Brew](https://www.raycast.com/nhojb/brew)
- [CleanShot X](https://www.raycast.com/Aayush9029/cleanshotx)
- [Raindrop.io](https://www.raycast.com/lardissone/raindrop-io)
- [TinyPNG](https://www.raycast.com/kawamataryo/tinypng)
- [Visual Studio Code](https://www.raycast.com/thomas/visual-studio-code)
- [Youtube](https://www.raycast.com/tonka3000/youtube)
<br>

### [AMETHYST](https://ianyh.com/amethyst/) - Window Management
<br>

### MENU BAR
#### [SYSTEM STATS](https://github.com/exelban/stats) - CLock & Widgets
- Widgets:
  - Clock (Allows you to show many different timezones)
    | **Name** | **Format** | **Time Zone** |
    |:----------|:----------:|:----------|
    | Home | HH:mm | UTC -4 |
    | Vancouver (Pacific) | yyyy-MM-dd HH:mm | UTC -7 |
    | Edmonton | yyyy-MM-dd HH:mm | UTC -6 |
    | Winnipeg (Central) | yyyy-MM-dd HH:mm | UTC -5 |
    | Halifax (Atlantic) | yyyy-MM-dd HH:mm | UTC -4 |
    | Hanoi | yyyy-MM-dd HH:mm | UTC +7 |
    | Seoul/Tokyo | yyyy-MM-dd HH:mm | UTC +9 |
  - Disable System Clock:
    - System Settings / Control Center / Menu Bar Only / Clock Options / Time
      - Style: Digital
  - Disk:
    - Widget: Bar Chart
      - Label: On
      - Frame: On
      - Color: Based on utilisation
  - RAM:
    - Widget: Bar Chart
      - Label: On
      - Frame: On
      - Color: Based on utilisation 
<br>

#### [ITSYCAL](https://www.mowglii.com/itsycal/) - Date & Calendar Widget
Replaces the date in the menu bar and shows a calendar widget when clicked-on.
- Settings:
  - General:
    - Launch at Login: Checked
    - Automatically Check for Updates: Checked
    - First Day of the Week: Monday
    - Event List Shows: 4 days
  - Appearance:
    - Menu Bar: 3rd icon
    - Format: `E, d MMM YYYY`
    - Hide Icon: Checked
  - Calendar:
    - Size: Biggest
    - Theme: Dark
    - Highlight: S, S
    - Show Events Dots: Checked
      - Use Colored Dots: Checked
    - Show Event Location: Checked
<br>

### SHELL, TERMINAL [iTerm2](https://iterm2.com/) & VSC 
#### ZSH
Using the `brew` version of ZSH (`/opt/homebrew/bin/zsh`) which is kept more up-to-date than Apple's version.

#### ITERM2
> *[Documentation](https://iterm2.com/documentation.html)*
Settings are saved with this repository (com.googlecode.iterm2.plist).

### [VISUAL STUDIO CODE(https://github.com/DeamonCorpse/VSC_Settings)
<br>

<hr>
<hr>
### ARC - Browser
I use the following extensions to stay productive:

* [Tabliss](https://tabliss.io/) - simple new tab page
* [OneTab](https://www.one-tab.com/) - consolidate a bunch of open tabs into a shareable list of links
* [Dark Reader](https://darkreader.org/) - turn any site into dark mode

I use the following extensions to protect my privacy while browsing the web:

* Adblocker - [uBlock Origin](https://github.com/gorhill/uBlock)
* Tracker Blocker - [Privacy Badger](https://privacybadger.org/)
  * Firefox now includes tracker blocking, but I leave Privacy Badger enabled.
* [Decentraleyes](https://decentraleyes.org/)
  * Caches CDN links locally and intercepts requests to serve from the cache. Prevents CDNs from tracking you across websites.
<br>

### SETAPP APPLICATIONS
The following apps are installed through setapp:
- Airbuddy: Monitor your wireless devices
- Bartender: Personalize your menu bar
- CleanMyMac X: Speed up and decluter your Mac
- CleanShot X: Take better screen shots and GIFs
- Forklift: Manage files across servers
- Sip: Pick colors for your designs
- PDF Squeezer: Compress PDFs without quality loss
<br>
