# macOS Stuff

Many of these commands will be applicable to different UNIX environments

to show hidden files:
    `defaults write com.apple.finder AppleShowAllFiles -bool TRUE` 

Download file using curl:
    `curl -O [file URL]` 

Overwrite sleep settings:
    `caffeinate -u -t [seconds]` 

Enable character repeat (important for VIM Plugins):
    `defaults write -g ApplePressAndHoldEnabled -bool FALSE` 

Change directory screenshots are saved to:
    `defaults write com.apple.screencapture location [dir]` 

Allow anyone to read/write a file:
    `sudo chmod 777 [file]`

Allow anyone to only read a file:
    `sudo chmod 644 [file]`

Set ownership of file to user:
    `sudo chmod [username] [file]`


## Setup
- Clone dotfiles into `~/dotfiles` and create systemlinks
- Dark Mode (including Dark Reader)
- Setup iCloud Sync for `~/desktop` and `~/documents`


### Dotfile System-links
- `.config`
- `.init.vim`
- `.nvim`
- `.vim`
- `.vimrc`
- `.tmux.conf`
- `.zshrc`

## Essential homebrew formulas
- coreutils
- ffmpeg
- fzf
- zsh
- git
- htop
- mpv
- openssl
- neovim
- vim
- tmux
- python
- python3
- streamlink
- youtube-dl


## Applications
- Alfred
- Things
- Spark
- iTerm
- PDF Expert
- Tyme
- 1password
- Screens 4
- Little Snitch
- Bartender
- iStat Menus
- Carbon Copy Cloner
