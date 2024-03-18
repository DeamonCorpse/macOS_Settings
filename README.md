# macOS SETTINGS

This repo contains info on all the apps / tools / settings I use on my Mac.

What Macbook do I have?
OS Settings
Desktop
Finder
Dock
Quick Launching
Homebrew
Homebrew
RayCast Homebrew Plugin
Window Management
App Switching
Menu Bar Utilities
Hidden Bar
System Stats Widgets
Menu Bar Calendar
Break Timer
Web Browser
Firefox
Other Apps I Use Daily
Docker
Terminal
Shell
Load dotfiles
Github SSH Setup
Other command line tools I use
Node.js
Global Modules
VS Code
What Macbook do I have?
I am using a 2020 13" Macbook Pro for work and a 2021 14" Macbook Pro for personal stuff.

The specs for both machines:

2020
Apple M1
2021
Apple M1 Pro
16GB RAM
500GB SSD
Read more about these Macbooks here:

2020
2021
OS Settings
These are my preferred settings for Desktop, Finder and the Dock.

Desktop
I don't like the new Desktop, Stage Manager or Widget features in Sonoma, so I disable them.

System Preferences
Desktop & Dock
Desktop & Stage Manager
Show Items
On Desktop -> uncheck
In Stage Manager -> uncheck
Click wallpaper to reveal desktop -> Only in Stage Manager
Stage Manager -> uncheck
Widgets
On Desktop -> uncheck
In Stage Manager -> uncheck
Finder
Finder -> Preferences
General -> Show these on the desktop -> Select None
I try to keep my desktop completely clean.
General -> New Finder windows show -> Home Folder
I prefer to see my home folder in each new finder window instead of recent documents
Advanced -> Show all filename extensions -> Yes
Advanced -> Show warning before changing an extension -> No
Advanced -> When performing a search -> Search the current folder
View
Show Status Bar
Show Path Bar
Show Tab Bar
Dock
I don't use the Dock at all. It takes up screen space, and I can use RayCast to launch apps and AltTab to switch between apps. I make the dock as small as possible and auto hide it.

System Preferences
Desktop & Dock
Size -> Small as possible
Position on screen -> Left
Automatically hide and show the Dock -> Yes
Animate opening applications -> No
Show suggested and recent apps in the Dock -> No
Quick Launching
The built in spotlight search is a bit slow for me and usually has web search results as the default instead of apps or folders on my machine.

I recently switched from Alfred to RayCast. I'm really liking it so far.

brew install raycast
Homebrew
Homebrew
Homebrew allows us to install tools and apps from the command line.

To install it, open up the built in Terminal app and run this command:

/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
This will also install the xcode build tools which is needed by many other developer tools.

After Homebrew is done installing, we will use it (via RayCast) to install everything else we need.

RayCast Homebrew Plugin
Install the RayCast Homebrew Plugin so we can easily install formulae and casks directly from RayCast.

Window Management
I know this feature is built in to a lot of other operating systems, but it is not built in to a Mac, so we need an app for it.

RayCast has this feature built in, but I am still using a separate app for this.

I use rectangle to move and resize windows using keyboard shortcuts. I used to use spectacle, but rectangle is more regularly maintained and allows me to use all of the same keyboard shortcuts as spectacle.

I highly recommend installing this and memorizing the keyboard shortcuts. Fluid and seamless window management is key to being productive while coding.

Search for rectangle in RayCast brew search or:

brew install rectangle
App Switching
The built in App switcher only shows application icons, and only shows 1 icon per app regardless of how many windows you have open in that app.

I use an app switcher called AltTab. It shows full window previews, and has an option to show a preview for every open window in all applications (even minimized ones).

I replace the built-in CMD+TAB shortcut with AltTab.

Search for alt-tab in RayCast brew search or:

brew install alt-tab
Menu Bar Utilities
Hidden Bar
If you have several apps running that have menu bar icons, Hidden Bar will let you choose which ones should be hidden after a timeout. This cleans things up if you have a ton of background apps running.

Search for hiddenbar in RayCast brew search or:

brew install hiddenbar
System Stats Widgets
I use stats to see my network traffic, CPU temp / usage and RAM usage at a glance.

In each widget, a key setting to look for is under "widget settings", choose "merge widgets into one".

Search for stats in RayCast brew search or:

brew install stats
Menu Bar Calendar
I like to have a calendar in the menu bar that I can quickly look at. stats does not include one, so I found itsycal.

brew install itsycal
itsycal shows the date, so I hide the date in the system menu bar widget:

System Preferences
Dock & Menu Bar
Clock
Show Date -> Never
Show Day of Week -> No
Break Timer
I use an app called Time Out.

I have it setup to show:

10 second micro break every 15 minutes
5 minute long break every 60 minutes
There is also a cross platform break timer call Stretchly. I have not used it but a lot of people have recommended it.

Web Browser
Firefox
I use Firefox because it is open source and comes from the Mozilla Foundation, a non profit company that respects my privacy.

I use Firefox Developer Edition. To install this with brew you will need to tap a cask first:

brew tap homebrew/cask-versions
You can then install Firefox Developer Edition with brew:

brew install homebrew/cask-versions/firefox-developer-edition
I use the following extensions to stay productive:

Tabliss - simple new tab page
OneTab - consolidate a bunch of open tabs into a shareable list of links
Dark Reader - turn any site into dark mode
I use the following extensions to protect my privacy while browsing the web:

Adblocker - uBlock Origin
Tracker Blocker - Privacy Badger
Firefox now includes tracker blocking, but I leave Privacy Badger enabled.
Decentraleyes
Caches CDN links locally and intercepts requests to serve from the cache. Prevents CDNs from tracking you across websites.
Other Apps I Use Daily
android-file-transfer - Transfer files to / from my android phone
android-platform-tools - Installs adb without the need for the full android studio.
keepingyouawake - Prevents my Mac from going to sleep when I'm presenting / live streaming
discord - Messaging / Community
vlc - I use VLC to watch videos instead of the built in QuickTime.
keka - Can extract 7z / rar and other types of archives
kap - Screen recorder / gif maker
figma - Image editor
visual-studio-code - Code Editor
sublime-text - Note taking (I know there are better apps...)
You can install them in one go by placing them all into a text file and then running brew install:

android-file-transfer
android-platform-tools
keepingyouawake
discord
slack
vlc
keka
kap
time-out
figma
visual-studio-code
sublime-text
insomnia
xargs brew install < apps.txt
Docker
There are multiple results when you search docker within brew. To install Docker desktop:

brew install --cask docker
Terminal
I prefer iTerm2 because:

Lots of customization options
Clickable links
Native OS notifications
There are a lot of options for a terminal replacement, but I've been using iTerm2 for years and it works great for my needs.

Checkout their documentation for more info on what iTerm2 can do: https://iterm2.com/documentation.html

brew install iterm2
Once installed, launch it and customize the settings / preferences to your liking. These are my preferred settings:

Appearance
Theme
Minimal
Profiles
Default
General -> Working Directory -> Reuse previous session's directory
Colors -> Basic Colors -> Foreground -> Lime Green
Text -> Font -> Anonymous Pro
You can download this font here.
I use this font in VS Code as well
Text -> Font Size -> 36
I use my Macbook to present / teach, so a big font size is important so everyone can see the commands I'm typing
Keys -> Key Mappings -> Presets -> Natural Text Editing
This allows me to use the keyboard shortcuts I know and love inside of iTerm2
Shell
Mac now comes with zsh as the default shell. I've switched to using this with Oh My Zsh.

Load dotfiles
All my dotfiles are stored on github.

I clone this repo to my machine and copy the files into my home directory.

Github SSH Setup
Follow this guide to setup an ssh key for github
Follow this guide to add the ssh key to your github account
Other command line tools I use
ffmpeg - edit videos from the command line
imagemagick - edit images from the command line
brew install ffmpeg
brew install imagemagick
Node.js
I use nvm to manage the installed versions of Node.js on my machine. This allows me to easily switch between Node.js versions depending on the project I'm working in.

See installation instructions here.

OR run this command (make sure v0.39.7 is still the latest)

curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.7/install.sh | bash
Now that nvm is installed, you can install a specific version of node.js and use it:

nvm install 20
nvm use 20
node --version
Global Modules
There are a few global node modules I use a lot:

lite-server
Auto refreshing static file server. Great for working on static apps with no build tools.
http-server
Simple static file server.
license
Auto generate open source license files
gitignore
Auto generate .gitignore files base on the current project type
npm install -g lite-server http-server license gitignore
VS Code
VS Code is my preferred code editor.

You can view all of my VS Code settings / extensions here.
