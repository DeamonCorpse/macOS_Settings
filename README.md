# macOS SETTINGS
Info on all the apps / tools / settings used on my Mac.
<br>

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
- **Menu Bar Only**
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
- **Desktop & Stage Manager**
  - Show Items
    - On Desktop -> On
  - Click wallpaper to reveal desktop -> Only in Stage Manager
  - Widgets
    - Show Widgets On Desktop -> On
    - Widget Style: Full Color
    - Use iPhone Widgets: On
  - Default Web Browsere: Arc
  - **Windows**
    - Prefer Tabs when Opening Documents: Always
    - Ask to Keep Changes when CLosing Documents: On
    - Close Windows when Quitting an Application: On
  - **Mission Control**
    - Group Windows by Application: On
  - **Hot Corners**
    - Top Left: ⌥ Start Screen Saver
    - Bottom Left: ⌥ Put Display to Sleep
    - Top Right: ⌥ Notification Center
    - Bottom Right: ⌥ Quick Note
<br>

## macOS APPLICATIONS
### FINDER SETTINGS
- General
  - Show these on the Desktop: External Disks
  - New Finder Windows Show: Downloads
  - Open Folders in Tabs Instead of New Windows: Checked
- Tags: Evedrything Unchecked
- Sidebar:
  - Checked: Applications, Downloads, Home iCloud Drive, Desktop, Hard Disks, External Disks, Cloud Storage, Bonjour Computers, Connected Servers
- Advanced
  - Show all filename extensions: Checked
  - Show warning before changing an extension: Checked
  - Remove Items from the Trash After 30 Days: Checked
  - When Performing a Search: Search the Current Folder
- View
  * As List
  * Sort By: Name
  * Show Toolbar
  * SHow Path Bar
  * Show Status Bar
<br>

## 3RD PARTY APPLICATIONS
### HOMEBREW
[Homebrew](https://brew.sh/) is dubbed as the missing macOS package manager and allows us to install tools and apps from the command line.

- It can be installed by using the command on the brew homepage. *It will also install Apple's 'Xcode' tools as a dependency.*
- Once Installed, run the following commands to install all casks (applications) and formulae (cli tools):

```sh
xargs brew install < brew_casks.txt
xargs brew install < brew_formulae.txt
```
<br>

## RAYCAST (replacing quick launch)
*Raycast is installed as a cask by `homebrew`*<br>
Quick Launch is replaced by [RayCast](https://www.raycast.com/).


<hr>
<hr>



### RayCast Homebrew Plugin

Install the [RayCast Homebrew Plugin](https://www.raycast.com/nhojb/brew) so we can easily install formulae and casks directly from RayCast.

## Window Management

I know this feature is built in to a lot of other operating systems, but it is not built in to a Mac, so we need an app for it.

RayCast has this feature built in, but I am still using a separate app for this.

I use [rectangle](https://rectangleapp.com/) to move and resize windows using keyboard shortcuts. I used to use [spectacle](https://www.spectacleapp.com/), but rectangle is more regularly maintained and allows me to use all of the same keyboard shortcuts as spectacle.

I highly recommend installing this and memorizing the keyboard shortcuts. Fluid and seamless window management is key to being productive while coding.

Search for `rectangle` in RayCast `brew search` or:

```
brew install rectangle
```

## App Switching

The built in App switcher only shows application icons, and only shows 1 icon per app regardless of how many windows you have open in that app.

I use an app switcher called [AltTab](https://alt-tab-macos.netlify.app/). It shows full window previews, and has an option to show a preview for every open window in all applications (even minimized ones).

I replace the built-in `CMD+TAB` shortcut with AltTab.

Search for `alt-tab` in RayCast `brew search` or:

```sh
brew install alt-tab
```

## Menu Bar Utilities

### Hidden Bar

If you have several apps running that have menu bar icons, [Hidden Bar](https://github.com/dwarvesf/hidden) will let you choose which ones should be hidden after a timeout. This cleans things up if you have a ton of background apps running.

Search for `hiddenbar` in RayCast `brew search` or:

```sh
brew install hiddenbar
```

### System Stats Widgets

I use [stats](https://github.com/exelban/stats) to see my network traffic, CPU temp / usage and RAM usage at a glance.

In each widget, a key setting to look for is under "widget settings", choose "merge widgets into one".

Search for `stats` in RayCast `brew search` or:

```sh
brew install stats
```

### Menu Bar Calendar

I like to have a calendar in the menu bar that I can quickly look at. stats does not include one, so I found [itsycal](https://www.mowglii.com/itsycal/).

```sh
brew install itsycal
```

itsycal shows the date, so I hide the date in the system menu bar widget:

* System Preferences
  * Dock & Menu Bar
      * Clock
          * Show Date -> Never
          * Show Day of Week -> No

## Break Timer

I use an app called [Time Out](https://www.dejal.com/timeout/).

I have it setup to show:
* 10 second micro break every 15 minutes
* 5 minute long break every 60 minutes

There is also a cross platform break timer call [Stretchly](https://hovancik.net/stretchly/). I have not used it but a lot of people have recommended it.

## Web Browser

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
