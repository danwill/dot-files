# Dan's dotfiles

Borrowed from https://github.com/driesvints/dotfiles

OSX Settings from https://github.com/mathiasbynens/dotfiles/blob/master/.macos

https://getgrav.org/blog/macos-catalina-apache-multiple-php-versions

Install XCode, used by Homebrew:
```
xcode-select --install
```

Install Homebrew
```
$ /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

Check Homebrew
``` 
brew doctor
```


## Show me what you got

### Command Line
* [AWS CLI](https://docs.aws.amazon.com/cli/latest/reference/)
* `bat` - `cat` with syntax highlighting
* `http` - [httpie](https://httpie.org/), a HTTP client for testing HTTP calls in the command line. 
    - `http -f POST example.org hello=World`
* `mackup` - [mackup](https://github.com/lra/mackup), backup and restore applications settings
    - `mackup backup`
    - `mackup restore`
* `mas` - [Mac App Store](https://github.com/mas-cli/mas), install App Store apps via CLI
    - `mas list`
    - `mas serach Dash`
    - `mas install [app-identifier]`
* `tree` - [tree listing](http://mama.indstate.edu/users/ice/tree/tree.1.html) 

### Development
* Image optimizers: `jpegoptim`, `optiping`, `pngquant`, `svgo`, `gifsicle`
* `php` is installed via brew, and defaults to the latest version. Can use Laravel Valet to switch active version (valet is installed in `install.sh`).
    -  `valet use php@7.2`
* `wp-cli` for Wordpress commands
* mysql 5.7 - by default, set up at 127.0.0.1 with a username of `root` and a blank password


### Apps

#### Productivity
* Alfred
* Divvy
* Evernote
* Fontbase - Font manager
* Slack
* Numi - natural language calculator
* The unarchiver

#### Customization
* [Aerial](https://github.com/JohnCoates/Aerial) - Apples aerial videos as screensaver

#### Backup and Security
* 1Password
* Backblaze
* Dropbox

#### 3D Printing
* Fusion 360
* Prusa Slicer
* Cura

#### Development
* [Brew Servies Menubar](https://github.com/andrewn/brew-services-menubar)
* [Caffeine](http://lightheadsw.com/caffeine/) - Prevent macbook from going to sleep
* [Contraste](https://contrasteapp.com/) - Accessibility contrast checker
* [Dash](https://kapeli.com/dash) - API documentation browwser
* ImageOptim
* Firefox
* Chrome
* Opera
* Figma
* iTerm 2
* [Insomnia](https://insomnia.rest/) - REST client (similar to Postman)
* [Pixelsnap](https://getpixelsnap.com/) - Ruler
* Sequel Pro
* Sketch
* Tower
* Transmit
* Vagrant
* Virtualbox
* VS Code


#### Other
* Discord
* Kap - screen recording
* OBS
* Steam
* VLC
* Winds - RSS Reader



## Installation

* Update macOS to the latest version with the App Store
* Install Xcode from the App Store, open it and accept the license agreement
* Install macOS Command Line Tools by running xcode-select --install
* Generate a new public and private SSH key and add them to Github
* Clone this repo to ~/.dotfiles
* Install Oh My Zsh
* Run install.sh to start the installation
* After mackup is synced with your cloud storage, restore preferences by running mackup restore
* Restart your computer to finalize the process
