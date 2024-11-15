# Loskir's macOS setup guide

Setting up a new macbook can be annoying. Here's a list of setting that I change when configuring macOS.

## Settings
### Appearance
- Show scroll bars - when scrolling

### Desktop
- Screen saver - Hot corners - off

### Desktop & Dock
- Automatically hide and show - on
- Show recent - off

#### Mission control
- Automatically rearrange - off
- When switching - off
- Group windows - on

### Keyboard
- Key Repeat - fast
- Delay - second shortest
- Globe key — Do Nothing
#### Keyboard Shortcuts
- Spotlight - off (for Raycast)
- Input sources - select previous - off
- Input sources - select next - F13 (for Karabiner)
- Screenshots - assign "clipboard" variants without ctrl (⌘⇧4 etc.)
#### Text Input → Edit → All Input Sources
- Correct spelling - off
- Capitalize - off
- Add period with double-space - off
- Use smart quotes and dashes - off

### Trackpad
- Tracking speed - 5th from right
- More gestures - swipe between pages - Off
- More gestures - expose - Swipe Down with Three Fingers

### Battery
- Options... → Slightly dim - off

## [TinkerTool](https://www.bresink.com/osx/TinkerTool.html)
### Dock
- Disable delay
- Minimizer effect - suck in
- Enable slow motion

### General
- Keyboard - support key repeat

### Font Smoothing - off

## Finder → Settings
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
- `sudo nano /etc/pam.d/sudo_local` -> Add `auth sufficient pam_tid.so` to the beginning to enable touch id auth for sudo.
- Install [brew](https://brew.sh/)
- `brew install stats` (https://github.com/exelban/stats)
- `brew install micro` (https://micro-editor.github.io/)
- `brew install fnm` (https://github.com/Schniz/fnm)

### Disable input source switch popup on Sonoma

`sudo defaults write /Library/Preferences/FeatureFlags/Domain/UIKit.plist redesigned_text_cursor -dict-add Enabled -bool NO`

## Other apps
- Install [Raycast](https://raycast.com). transfer config
- [velja](https://apps.apple.com/ru/app/velja/id1607635845?l=en&mt=12)
- [MonitorControl](https://github.com/MonitorControl/MonitorControl/releases)
- [Typography Layout](https://ilyabirman.ru/typography-layout/). How to remove default layout: [here](https://dev-postnov.ru/how-remove-the-default-keyboard-layout/)
