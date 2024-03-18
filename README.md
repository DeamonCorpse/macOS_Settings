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
  - Show Items
    - On Desktop -> On
  - Click wallpaper to reveal desktop -> Only in Stage Manager
  - Widgets
    - Show Widgets On Desktop -> On
    - Widget Style: Full Color
    - Use iPhone Widgets: On
  - Default Web Browsere: Arc
  - Windows:
    - Prefer Tabs when Opening Documents: Always
    - Ask to Keep Changes when CLosing Documents: On
    - Close Windows when Quitting an Application: On
  - **Mission Control**
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

### AMETHYST - Window Management
<br>

### MENU BAR
#### [SYSTEM STATS](https://github.com/exelban/stats)
- Widgets:
  - Clock (Allows you to show many different timezones)
    - Home: UTC -4
    - Vancouver (Pacific): UTC -7
    - Edmonton: UTC -6
    - Winnipeg (Central): UTC -5
    - Halifax (Atlantic): UTC -4
    - Hanoi: UTC +7
    - Seoul/Tokyo: UTC +9
  *Disable System Clock*:
    - System Settings/
  - Disk
  - RAM

<hr>
<hr>

#### [ITSYCAL](https://www.mowglii.com/itsycal/)
Replaces the date in the menu bar and shows a calendar widget when clicked-on.

* System Preferences
  * Dock & Menu Bar
      * Clock
          * Show Date -> Never
          * Show Day of Week -> No




### Firefox

I use Firefox because it is open source and comes from the [Mozilla Foundation](https://www.mozilla.org/en-US/about/manifesto/), a non profit company that [respects my privacy](https://www.mozilla.org/en-US/firefox/privacy/).

I use Firefox Developer Edition. To install this with `brew` you will need to tap [a cask](https://github.com/Homebrew/homebrew-cask-versions) first:

```sh
brew tap homebrew/cask-versions
```

You can then install Firefox Developer Edition with brew:

```sh
brew install homebrew/cask-versions/firefox-developer-edition
```

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

## Other Apps I Use Daily


* [keepingyouawake](https://keepingyouawake.app/) - Prevents my Mac from going to sleep when I'm presenting / live streaming
* [discord](https://discord.com/) - Messaging / Community
* [visual-studio-code](https://code.visualstudio.com/) - Code Editor




### Docker

There are multiple results when you search `docker` within `brew`. To install Docker desktop:

```sh
brew install --cask docker
```

## Terminal

I prefer [iTerm2](https://iterm2.com/) because:
* Lots of customization options
* Clickable links
* Native OS notifications

There are a lot of options for a terminal replacement, but I've been using iTerm2 for years and it works great for my needs.

Checkout their documentation for more info on what iTerm2 can do: [https://iterm2.com/documentation.html](https://iterm2.com/documentation.html)


```
brew install iterm2
```

Once installed, launch it and customize the settings / preferences to your liking. These are my preferred settings:

* Appearance
  * Theme
    * Minimal
* Profiles
  * Default
      * General -> Working Directory -> Reuse previous session's directory
      * Colors -> Basic Colors -> Foreground -> Lime Green
      * Text -> Font -> Anonymous Pro
          * You can download this font [here](https://www.marksimonson.com/fonts/view/anonymous-pro).
          * I use this font in VS Code as well
      * Text -> Font Size -> 36
          * I use my Macbook to present / teach, so a big font size is important so everyone can see the commands I'm typing
      * Keys -> Key Mappings -> Presets -> Natural Text Editing
          * This allows me to use the [keyboard shortcuts](https://gist.github.com/w3cj/022081eda22081b82c52) I know and love inside of iTerm2

### Shell

Mac now comes with `zsh` as the default [shell](https://en.wikipedia.org/wiki/Comparison_of_command_shells). I've switched to using this with [Oh My Zsh](https://ohmyz.sh/).

#### Load dotfiles

All my dotfiles are stored on [github](https://github.com/w3cj/dotfiles).

I clone this repo to my machine and copy the files into my home directory.

### Github SSH Setup

* Follow [this guide](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent) to setup an ssh key for github
* Follow [this guide](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account) to add the ssh key to your github account

#### Other command line tools I use

* [ffmpeg](https://en.wikipedia.org/wiki/FFmpeg) - edit videos from the command line
* [imagemagick](https://en.wikipedia.org/wiki/ImageMagick) - edit images from the command line

```sh
brew install ffmpeg
brew install imagemagick
```

## Node.js

I use nvm to manage the installed versions of Node.js on my machine. This allows me to easily switch between Node.js versions depending on the project I'm working in.

See installation instructions [here](https://github.com/nvm-sh/nvm#installing-and-updating).

OR run this command (make sure v0.39.7 is still the latest)

```sh
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.7/install.sh | bash
```

Now that nvm is installed, you can install a specific version of node.js and use it:

```sh
nvm install 20
nvm use 20
node --version
```

### Global Modules

There are a few global node modules I use a lot:

* lite-server
  * Auto refreshing static file server. Great for working on static apps with no build tools.
* http-server
  * Simple static file server.
* license
  * Auto generate open source license files
* gitignore
  * Auto generate `.gitignore` files base on the current project type

```
npm install -g lite-server http-server license gitignore
```

## VS Code

VS Code is my preferred code editor.

You can view all of my VS Code settings / extensions [here](https://github.com/CodingGarden/vscode-settings).
