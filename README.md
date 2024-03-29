# Loskir's macOS setup guide

Setting up a new macbook can be annoying. Here's a list of setting that I change when configuring macOS.

## Settings
### General
- Show scroll bars - when scrolling

### Desktop
- Screen saver - Hot corners - off

### Dock and menu bar
- Automatically hide and show - on
- Show recent - off

### Mission control
- Automatically rearrange - off
- When switching - off
- Group windows - on

### Keyboard
- Key Repeat - fast
- Delay - second shortest
#### Text
- Correct spelling - off
- Capitalize - off
- Add period - off
- Smart quotes - off
#### Shortcuts
- Spotlight - off (for Raycast)
- Input sources - select previous - `ctrl+space`
- Screenshots - assign "clipboard" variants without ctrl (⌘⇧4 etc.)

### Trackpad
- Tracking speed - 5th from right
- More gestures - swipe between pages - off
- More gestures - expose - on

### Battery
- Slightly dim - off

## [TinkerTool](https://www.bresink.com/osx/TinkerTool.html)
### Dock
- Disable delay
- Minimizer effect - suck in
- Enable slow motion

### General
- Keyboard - support key repeat

### Font Smoothing - off

## Finder
### Sidebar
- home dir - on
### Advanced
- Show all extensions - on
- Search - current folder
- Folders on top - in windows - on

## Telegram (swift ver)
### General
- Show calls tab - off
- Show icon in menu bar - off
- Force touch action - edit

### Data and Storage
- Storage limit - 5gb

## Activity monitor
- View - Update Frequency - Very often

## Shell
- `sudo nano /etc/pam.d/sudo` -> Add `auth sufficient pam_tid.so` to the beginning to enable touch id auth for sudo.
- Install [brew](https://brew.sh/)
- `brew install stats` (https://github.com/exelban/stats)
- `curl https://getmic.ro | bash; sudo mv ./micro /usr/local/bin` (https://micro-editor.github.io/)
- Install [fnm](https://github.com/Schniz/fnm)

### Disable input source switch popup on Sonoma

`sudo defaults write /Library/Preferences/FeatureFlags/Domain/UIKit.plist redesigned_text_cursor -dict-add Enabled -bool NO`

## Other apps
- Install [Raycast](https://raycast.com). transfer config
- [velja](https://apps.apple.com/ru/app/velja/id1607635845?l=en&mt=12)
- [MonitorControl](https://github.com/MonitorControl/MonitorControl/releases)
- [Typography Layout](https://ilyabirman.ru/typography-layout/). How to remove default layout: [here](https://dev-postnov.ru/how-remove-the-default-keyboard-layout/)
