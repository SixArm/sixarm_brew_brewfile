##
# SixArm Brew Brewfile
#
# We use this Brewfile for our teams and their developer laptops.
#
# This file installs many apps, including office suites, multimedia suites,
# programming langauges and IDEs, unix utilities, and sysadmin tools.
#
# This file is organized in meaningful sections because we want to
# make it easy for you to pick and choose sections that you want.
#
# ## Taps
#
# We do not use tap in this file; instead, we use full paths.
# This is because we want to be as clear as possible about what
# is being installed, and from what locations.
#
# ## Dupes
#
# We generaly prefer homebrew/dupes to preinstalled Mac software.
# For example, we prefer the GNU `sed` command vs. macOS `sed` command.
# However, we have seen this cause conflicts with macOS software that
# isn't aware of GNU; therefore we install the dupes in parallel.
#
# ## Contents
#
# This file has a bunch of sections:
#
#   * Browsers: firefox, google-chrome, opera, ...
#   * Passwords: keybase, 1password, lastpass, ...
#   * Terminals: iterm2, tmux, screen, ...
#   * Shells: bash, zsh, fish, mosh, ...
#   * Editors: vim, emacs, atom, sublime, ...
#   * Downloaders: curl, wget, cask, carthage, ...
#   * Version control: git, hg, svn, cvs, ...
#   * GNU command line tools
#   * System related: TODO
#   * File compression: zstd, unrar, unzip, ...
#   * File synchronization: rsync, unison, syncthing, ...
#   * Text search: ripgrep, ag, sift, ...
#   * Operating-related
#   * Build tools
#   * Database servers: postgresql, redis, ...
#   * Database searchers: sphinx, TODO
#   * Database managers: TODO
#   * Markup languages: pandoc, TODO
#   * Programming languages: Java, Node, Python, ...
#
# ## See Also
#
# See also:
#
#   * https://www.topbug.net/blog/2013/04/14/install-and-use-gnu-command-line-tools-in-mac-os-x/
#
# ## Tracking
#
# * Package: sixarm_brew_brewfile
# * Version: 2.2.0
# * Created: 2017-01-01
# * Updated: 2019-01-04T01:54:45Z
# * License: GPL
# * Contact: Joel Parker Henderson (joel@joelparkerhenderson.com)
##

##
# Browsers
#
# We prefer Firefox because it's open source.
##

# Firefox web browser
cask 'firefox'

# Google Chrome web browser
cask 'google-chrome'

# Opera web browser
#cask 'opera'

# Brow.sh text browser
#tap 'browsh-org/homebrew-browsh'
#brew 'browsh'

##
# Passwords
#
# We use password-manager applications with many of our projects.
# If you don't use these, feel free to delete them.
##

# Pass, a Unix password manager
brew 'pass'

# Keybase.io digital signature manager
brew 'keybase'

# 1password is a password manager
cask '1password'

# LastPass is a password manager
cask 'lastpass'

##
# Terminals
#
# We typically use `tmux` and `tmate`,
# and sometimes fall back on `screen`.
##

# iTerm is our favorite terminal app.
cask 'iterm2'

# bat is like `cat` plus line numbers, syntax highlighting, and more.
brew 'bat'

# tmux is a newer terminal multiplexer.
#
# TODO:
#
#     brew 'pkg-config' && brew link pkg-config && brew 'tmux'
#
brew 'tmux'

# tmate is a fork of tmux that makes screen sharing friendlier.
brew 'tmate'

# Screen is an older terminal multiplexer.
brew 'homebrew/dupes/screen'

# ngrok creates a secure tunnels to localhost
brew 'ngrok'

##
# Shells
#
# We typically use bash, zsh, fish, and mosh.
##

# Bash is the Bourne Again SHell. Bash is an sh-compatible shell.
brew 'bash'

# Programmable completion functions for bash
brew 'bash-completion'

# Bashish is a theme enviroment for text terminals.
brew 'bashish'

# Zsh is a shell designed for interactive use.
brew 'zsh'

# Fish shell.
brew 'fish'

# Mobile Shell (MOSH) is like SSH plus roaming and smart echo.
brew 'mobile-shell'

##
# Editors
#
# We typically use command line editors (vim, emacs, etc.)
# and sometimes use GUI editors (atom, sublime, etc.)
##

# Vim editor
brew 'vim'

# MacVIM editor
cask 'macvim'

# Emacs editor
cask 'emacs-plus'

# Emacs editor for Spacemacs
# TODO: brew tap d12frosted/emacs-plus
brew 'emacs-plus'
# brew linkapps emacs-plus

# Atom editor by GitHub
cask 'atom'

# Sublime text editor
cask 'sublime-text'

# GNU Aspell is a free open source spell checker; compare `lspell`.
#brew 'aspell --with-lang=en'

# Enca - detect and convert encoding of text files
brew 'enca'

# MacTex: LaTeX document preparation system with high-quality typesetting.
cask 'mactex'

##
# Downloaders
#
# These items download files and fetch content from the network.
##

# Carthage is a simple, decentralized dependency manager for Cocoa
brew 'carthage'

# Homebrew Cask extends Homebrew to install OS X applications and large binaries.
brew 'cask'

# curl is a command line tool for transferring data with URL syntax
brew 'curl'

# HTTrack is a free and easy-to-use offline browser utility.
brew 'httrack'

# Wget is a free software package for retrieving files using HTTP and FTP.
brew 'wget'

# GNU inetutils contains telnet, ftp, etc.
brew 'inetutils'

##
# Version control
#
# We prefer `git` version control. We also work on a wide
# range of systems, so we also sometimes use CVS, HG, and SVN.
##

# CVS is a version control system.
brew 'cvs'

# Git is a free and open source distributed version control system.
#
# TODO: why do we need brew 'git' and also cask 'git'?
brew 'git'
cask 'git'

# Git Large File Storage for adding text pointers to external data.
brew 'git-lfs'

# TODO
brew 'git-cola'

# Git extras: utilities including summary, repl, population, etc.
cask 'git-extras'

# Git extensions to provide high-level operations for Git Flow branching model.
brew 'git-flow'

# TODO
brew 'git-ftp'

# TODO
brew 'git-gerrit'

# TODO
brew 'git-multipush'

# TODO
brew 'git-now'

# TODO
brew 'git-url-sub'

# GitUp friendly Git interface and visualizer
cask 'gitup'

# SourceTree graphic client for git
cask 'sourcetree'

# Mercurial version control system.
brew 'hg'

# Subversion version control system.
#
# TODO: brew 'sqlite' && brew 'subversion'
brew 'subversion'

##
# GNU command line tools
#
# If you are moving onto macOS from GNU/Linux, then you would probably
# find out that the command line tools shipped with macOS are not as
# powerful and easy to use as the tools in Linux. The reason is that
# macOS uses the BSD version command line tools, which are different
# from the Linux version.
#
# Note: if you choose to replace the macOS commands with GNU commands,
# then be aware that you may have some compatibility issues with shell
# scripts written specifically for macOS.
#
# If you like using man pages, then you may also want to add an
# itemto the to the MANPATH environmental variable:
#
#     $HOMEBREW_PREFIX/opt/coreutils/libexec/gnuman
#
# For more about the GNU command line tools and brew, see this:
# https://www.topbug.net/blog/2013/04/14/install-and-use-gnu-command-line-tools-in-mac-os-x/
##

# Basic file, shell and text manipulation utilities of the GNU operating system.
brew 'coreutils'

brew 'binutils'
brew 'diffutils'
brew 'ed'
brew 'findutils'
brew 'gawk'
brew 'gnu-indent'
brew 'gnu-sed'
brew 'gnu-tar'
brew 'gnu-which'
brew 'gnutls'
brew 'gzip'
brew 'watch'
brew 'wdiff'

##
# Some GNU command line tools already exist by default on OS X.
# We choose to replace these with newer versions.
##

brew 'gdb'  # gdb requires further actions to make it work. See `brew info gdb`.
brew 'gpatch'
brew 'less'
brew 'm4'
brew 'make'
brew 'nano'

##
# System related
#
# These are fundamental operating system tools that we use often.
##

# Automake is a tool for automatically generating Makefile installation files.
brew 'automake'

# GNU Privacy Guard (GnuPG) provides encryption as a free replacement for PGP.
brew 'gpg'

# GNU Privacy Guard (GnuPG) PIN entry for macOS to do GPG terminal decryption
brew 'pinentry-mac'

# OpenSSL is an open-source implementation of the SSL and TLS protocols.
brew 'openssl'

# pkg-config is a helper tool used when compiling applications and libraries.
brew 'pkg-config && brew link pkg-config && brew install tmux'

# Functions for use by applications that allow users to edit command lines while typing.
brew 'readline'

# Parallel SSH
brew 'pssh'

# pkg-config is a helper tool used when compiling applications and libraries.
brew 'pkg-config'

# PCRE: Perl-compatible regular expressions, for better searching.
brew 'pcre'
brew 'pcre++'

# fd: a simple, fast and user-friendly alternative to find.
brew 'fd'

##
# File compression/uncompression
#
# We prefer `zstd` because it is the best modern compression.
##

# Zstandard is the best modern compression
brew 'zstd'

# WinRAR provides compression/decompression for RAR and ZIP files.
brew 'unrar'

# unzip is the classic command.
brew 'homebrew/dupes/unzip'

##
# File synchronization
#
# We use `rsync` for our systems administration,
# and a variety of web-based services for file sharing.
##

# rsync is the classic unix file synchronizer.
brew 'homebrew/dupes/rsync'

# Unison is a high-level file synchronization utility.
brew 'unison'

# Syncthing is open source file sharing.
brew 'syncthing'

# BitTorrent Sync is closed source file sharing.
cask 'bittorrent-sync'

# Dropbox file sharing.
cask 'dropbox'

# Transmission bittorrent client.
cask 'transmission'

# Box.com sync
cask 'box-sync'

##
# Text search
#
# We prefer ripgrep because it is very fast and very safe.#
##

# ripgrep is text search; we prefer it over grep, ag, git grep, ucg, pt, sift.
brew 'https://raw.githubusercontent.com/BurntSushi/ripgrep/master/pkg/brew/ripgrep.rb'

# grep is the classic searcher
brew 'grep'

# ag is "the silver searcher" search tool; retired by ripgrep.
brew 'ag'

# sift is like grep, plus faster and with more features; retired by ripgrep.
brew install sift

# xsv is for CSV file parsing, and is fast, full featured, and flexible.
brew 'xsv'

# Tad is CSV viewer with features for pivot, search, etc.
cask 'tad'

# jq is a lightweight and flexible command-line JSON processor.
brew 'jq'

##
# Images
##

# GraphicsMagick is the swiss army knife of image processing.
brew 'graphicsmagick'

# TODO
brew 'graphviz'

# Gnuplot is a portable command-line driven graphing utility.
brew 'gnuplot'

# yEd is desktop application to generate high-quality diagrams.
cask 'yed'

##
# Server-Related
##

# Docker software containers to help distribute applications.
brew 'docker'

# Compose is a tool for defining and running multi-container Docker applications.
brew 'docker-compose'

# Docker Machine installs Docker Engine on virtual hosts, and manages the hosts.
brew 'docker-machine'

# Consul tool for discovering and configuring services in your infrastructure.
brew 'consul'

# Monit is for managing and monitoring Unix systems.
brew 'monit'

# Nagios IT infrastructure monitoring.
brew 'nagios'

# NGINX web server.
brew 'nginx'

# Varnish reverse-proxy web application accelerator.
brew 'varnish'

##
# Font-Related
##

# Fontconfig is a library for configuring and customizing font access.
brew 'fontconfig'

# FreeType is a freely available software library to render fonts.
brew 'freetype'

# Command-line programs for manipulating fonts
brew 'lcdf-typetools'


##################### TODO ####################################


# TODO
brew 'html-xml-utils'

# TODO
brew 'lynx'

# Most is a powerful paging program; compare `less` and `more`.
brew 'most'

# Mutt is a small powerful text-based mail client.
brew 'mutt'

# Netcat is a networking utility for the TCP/IP protocol.
brew 'netcat'

# prettyping: ping with colorful output and progress bars
brew install prettyping

# TODO
brew 'ncdu'

# TODO
brew 'randomize-lines'

# TODO
brew 'rename'

# TODO
brew 'salt'

# Tree is a directory lister that shows a tree outline
brew 'tree'

# xclip is a command line interface to the X11 clipboard.
brew 'xclip'

## Media-Related

brew 'exif'
brew 'exiftags'
brew 'exiftool'
brew 'flac'
brew 'ffmpeg'
brew 'ffmpeg2theora'
brew 'ffmpegthumbnailer'
brew 'imagemagick'
brew 'kindle'
brew 'theora'

##
# Image-Related
##

brew 'libgphoto2'
brew 'libpng'
brew 'libtiff'

# Jasper command line transcoder between JPEG2000 and other formats.
brew 'jasper'


## Uncategorized

brew 'abook'
brew 'ack'
brew 'apachetop'
brew 'apple-gcc42'
brew 'ascii'
brew 'asciidoc'
brew 'asciitex'
brew 'autobench'
brew 'autoconf'
brew 'autoenv'
brew 'autogen'
brew 'autojump'
brew 'base64'
brew 'bcrypt'
brew 'bind'
brew 'bison'
brew 'bogofilter'
brew 'colordiff'
brew 'ctags'
brew 'docbook'
brew 'dovecot'
brew 'doxygen'
brew 'dpkg'
brew 'fakeroot'
brew 'findutils'
brew 'geoip'
brew 'gnu-barcode'
brew 'gnu-getopt'
brew 'gnu-indent'
brew 'gnu-prolog'
brew 'gnu-sed --default-names'
brew 'gnu-smalltalk'
brew 'gnu-tar'
brew 'gnu-time'
brew 'gnu-typist'
brew 'gnu-units'
brew 'gnu-which'
brew 'google-app-engine'
brew 'google-js-test'
brew 'google-perftools'
brew 'google-sparsehash'
brew 'google-sql-tool'
brew 'html2text'
brew 'htop'
brew 'httperf'
brew 'ical-buddy'
brew 'jmeter'
brew 'jpeg'
brew isntall libdnet
brew 'lzo'
brew 'rarian'
brew 'pixman'

# libMemcached is a client library and tools for the memcached server.
brew 'libmemcached'
brew 'memcached'

brew 'scrypt'
brew 'qt5'

# Tarsnap is a secure online backup service for Unix.
brew 'tarsnap'

# Valkyrie is a Qt4-based GUI for the Memcheck and Helgrind tools in Valgrind.
# Commented-out because it's currently incompatible with macOS 10.12.
#brew 'valkyrie'

# WINE runs Windows applications on other operating systems.
brew 'wine'

# Xapian is an open-source search engine library.
brew 'xapian'

##
# Dupes
#
# These formulas duplicate software provided by OS X,
# though may provide more recent or bugfix versions.
#
# We prefer to keep these explicitly listed in `/dupes`
# because these are potentially shadowing system tools,
# and we want to show that these are unusual and special.
#
# If you prefer to type less, then you can tap, like this:
#
#     brew tap homebrew/dupes
#
# Then you can install any forumla, such as:
#
#     brew 'awk'
#
##

brew 'homebrew/dupes/awk'
brew 'homebrew/dupes/diffstat'
brew 'homebrew/dupes/diffutils'
brew 'homebrew/dupes/ed'
brew 'homebrew/dupes/expect'
brew 'homebrew/dupes/fetchmail'
brew 'homebrew/dupes/file-formula'
brew 'homebrew/dupes/gdb'
brew 'homebrew/dupes/gpatch'
brew 'homebrew/dupes/gperf'
brew 'homebrew/dupes/grep'
brew 'homebrew/dupes/groff'
brew 'homebrew/dupes/gzip'
brew 'homebrew/dupes/heimdal'
brew 'homebrew/dupes/lapack'
brew 'homebrew/dupes/less'
brew 'homebrew/dupes/libedit'
brew 'homebrew/dupes/libiconv'
brew 'homebrew/dupes/libpcap'
brew 'homebrew/dupes/lsof'
brew 'homebrew/dupes/m4'
brew 'homebrew/dupes/make'
brew 'homebrew/dupes/nano'
brew 'homebrew/dupes/ncurses'
brew 'homebrew/dupes/openldap'
brew 'homebrew/dupes/openssh'
brew 'homebrew/dupes/screen'
brew 'homebrew/dupes/tcl-tk'
brew 'homebrew/dupes/tcpdump'
brew 'homebrew/dupes/tidy'
brew 'homebrew/dupes/units'
brew 'homebrew/dupes/whois'
brew 'homebrew/dupes/zlib'

##
# Brew cask enables installing typical Mac OS X applications.
# For example, these formulas may download a `*.dmg` file,
# then unpack it into the correct `/Applications` directory,
# and possibly configure the app with typical settings.
##

# Adium is an open source multi-protocol instant messaging client.
cask 'adium'

# TDB
cask 'adventure'

# TDB
cask 'alfred'

# TDB
cask 'amazon-cloud-drive'

# TDB
cask 'amazon-music'

# TDB
cask 'android-file-transfer'

# TDB
cask 'anki'

# AppCleaner thoroughly uninstalls unwanted apps.
cask 'appcleaner'

# TDB
cask 'arq'

# TDB
cask 'atext'

# TDB
cask 'audacity'

# TDB
cask 'backblaze-downloader'

# TDB
cask 'backuploupe'

# TDB
cask 'balsamiq-mockups'

# TDB
cask 'bartender'

# TDB
cask 'basecamp'

# TDB
cask 'beacon-scanner'

# TDB
cask 'blender'

# TDB
cask 'brain-workshop'

# TDB
cask 'cactus'

# TDB
cask 'caffeine'

# TDB
cask 'calibre'

# TDB
cask 'ccleaner'

# TDB
cask 'cheatsheet'

# TDB
cask 'chromecast'

# TDB
cask 'coconutbattery'

# TDB
cask 'codekit'

# TDB
cask 'commandq'

# TDB
cask 'dash'

# TDB
cask 'doxygen'

# TDB
cask 'duet'

# TDB
cask 'easysimbl'

# TDB
cask 'evernote'

# FileZilla FTP client
cask 'filezilla'

# Flash multimedia player
cask 'flash'

# TDB
cask 'fluid'

# Flux dims the screen colors for better nighttime visibility.
cask 'flux'

# TDB
cask 'freeplane'

# TDB
cask 'ganttproject'

# TDB
cask 'gfxcardstatus'

# GitHub source code social sharing
cask 'github'

# TDB
cask 'gitx'

###################

# TDB
cask 'grooveshark'

# TDB
cask 'harvest'

# TDB
cask 'hockey'

# TDB
cask 'hipchat'

# TDB
cask 'iterm2'

# TDB
cask 'joinme'

# TDB
cask 'jumpcut'

# Kindle book reader by Amazon
cask 'kindle'

# TDB
cask 'krita'

# TDB
cask 'launchy'

# TDB
cask 'little-snitch'

# LibreOffice is a large editor for text, spreadsheets, diagrams.
cask 'libreoffice'

# TODO
cask 'mysqlworkbench'

# TODO
cask 'p4merge'

# Pandora music player
cask 'pandora-one'

# TODO
cask 'paparazzi'

# Prezi slide show presentation.
cask 'prezi'

# TODO
cask 'pupil'

# TODO
cask 'quicksilver'

# Rdio music player.
cask 'rdio'

# TODO
cask 'rescuetime'

# Screenhero screen sharing by Slack.
cask 'screenhero'

# TODO
cask 'sequential'

# TODO
cask 'shortcat'

# Silverlight video player by Microsoft.
cask 'silverlight'

# TODO
cask 'skitch'

# Skype calling with video and phone calls.
cask 'skype'

# Discord chat
cask 'discord'

# Slack chat client
cask 'slack'

# TODO
cask 'sleep-monitor'

# Sophos anti virus
cask 'sophos-anti-virus-home-edition'

# TODO
cask 'sourcetree'

# Spotify music player
cask 'spotify'

# TODO
cask 'superduper'

# Synergy screen sharing utility
cask 'synergy'

# TODO
cask 'thisservice'

# Thunderbird email client by Mozilla.
cask 'thunderbird'

# TODO
cask 'transmit'

# TODO
cask 'todoist'

# TODO
cask 'todos'

# Unison file synchronizer.
cask 'unison'

# VLC media player
cask 'vlc'

##
# Extras
#
# These are packages that we may want.
#
# If you want any of these, please let us know,
# or create a pull request for this repository.
#
# Applications that we want that are not on brew:
#
#   * Kiwix
#   * SoapUI
#
# Applications that we want that we need to find:
#
#   * Automator
#   * Battery Health
#   * Cloud
#   * Coffitivity
#   * Disk Diag
#   * Docs for Xcode
#   * DxO Perspective
#   * Facebook
#   * Font Book
#   * Fotor
#   * Garmin
#   * Gmail
#   * Image Capture
#   * MailTab for Gmail
#   * Memory Clean
#   * MenuBar Stats
#   * Microsoft Remote Desktop
#   * Mint QuickView
#   * Prepo
#   * Screen Recorder Robot Lite
#   * Stickies
#   * Tab for Reddit
#   * The Unarchiver
#   * Time Machine
#   * Twitter
#   * VirtualDJ
#   * Wunderlist
#   * Xcode
#   * xScan
#
# Apple built-in apps:
#
#   * App Store
#   * Apple Configurator
#   * Calculator
#   * Calendar
#   * Chess
#   * Contacts
#   * DVD Player
#   * Dashboard
#   * Dictionary
#   * FaceTime
#   * Game Center
#   * GarageBand
#   * iBooks
#   * iCloud
#   * iMovie
#   * iPhoto
#   * iTunes
#   * iWork
#   * Keynote
#   * Launchpad
#   * Mail
#   * Maps
#   * Messages
#   * Mission Control
#   * Notes
#   * Numbers
#   * Pages
#   * Photo Booth
#   * Preview
#   * QuickTime Player
#   * Reminders
#   * Safari
#   * System Preferences
#   * TextEdit
##

# brew 'aws-cfn-tools'
# brew 'aws-cloudsearch'
# brew 'aws-elasticache'
# brew 'aws-iam-tools'
# brew 'aws-sns-cli'
# brew 'dart'
# brew 'json-c'
# brew 'json-glib'
# brew 'json_spirit'
# brew 'jsonpp'
# brew 'jstalk'
# brew 'jsvc'
# brew 'judy'
# brew 'justniffer'
# brew 'jython'
# brew 'kawa'
# brew 'kbtin'
# brew 'kdiff3'
# brew 'kelbt'
# brew 'kes'
# brew 'keychain'
# brew 'kismet'
# brew 'kite'
# brew 'kiwi'
# brew 'knife-completion'
# brew 'knock'
# brew 'konoha'
# brew 'ktoblzcheck'
# brew 'kumofs'
# brew 'kyoto-cabinet'
# brew 'kyoto-tycoon'
# brew 'kytea'
# brew 'lablgtk'
# brew 'lame'
# brew 'languagetool'
# brew 'lapack'
# brew 'lasi'
# brew 'lastfm_fplib'
# brew 'lastfmfpclient'
# brew 'lastfmlib'
# brew 'latex2html'
# brew 'latex2rtf'
# brew 'launch'
# brew 'lbdb'
# brew 'lcdf-typetools'
# brew 'lcov'
# brew 'lcrack'
# brew 'ldapvi'
# brew 'ldid'
# brew 'ldns'
# brew 'le'
# brew 'leafnode'
# brew 'ledger'
# brew 'ledit'
# brew 'legit'
# brew 'lemon'
# brew 'leptonica'
# brew 'less'
# brew 'lesspipe'
# brew 'lesstif'
# brew 'leveldb'
# brew 'lft'
# brew 'lftp'
# brew 'lha'
# brew 'libagg'
# brew 'libao'
# brew 'libarchive'
# brew 'libart'
# brew 'libass'
# brew 'libassuan'
# brew 'libbinio'
# brew 'libbs2b'
# brew 'libcaca'
# brew 'libcddb'
# brew 'libcdio'
# brew 'libcmph'
# brew 'libconfig'
# brew 'libcouchbase'
# brew 'libcroco'
# brew 'libcsv'
# brew 'libcue'
# brew 'libcuefile'
# brew 'libdaemon'
# brew 'libdap'
# brew 'libdbusmenu-qt'
# brew 'libdc1394'
# brew 'libdca'
# brew 'libdlna'
# brew 'libdmtx'
# brew 'libdnet'
# brew 'libdrizzle'
# brew 'libdshconfig'
# brew 'libdsk'
# brew 'libdv'
# brew 'libdvbpsi'
# brew 'libdvdcss'
# brew 'libdvdnav'
# brew 'libdvdread'
# brew 'libebml'
# brew 'libechonest'
# brew 'libelf'
# brew 'libemu'
# brew 'libev'
# brew 'libevent'
# brew 'libewf'
# brew 'libexif'
# brew 'libexosip'
# brew 'libextractor'
# brew 'libffi'
# brew 'libfishsound'
# brew 'libfixbuf'
# brew 'libflowmanager'
# brew 'libftdi'
# brew 'libgadu'
# brew 'libgaiagraphics'
# brew 'libgarmin'
# brew 'libgcrypt'
# brew 'libgda'
# brew 'libgee'
# brew 'libgeotiff'
# brew 'libgit2'
# brew 'libglade'
# brew 'libglademm'
# brew 'libgnomecanvas'
# brew 'libgpg-error'
# brew 'libgphoto2'
# brew 'libgsasl'
# brew 'libgsf'
# brew 'libgtextutils'
# brew 'libgtop'
# brew 'libharu'
# brew 'libhid'
# brew 'libical'
# brew 'libicns'
# brew 'libiconv'
# brew 'libid3tag'
# brew 'libident'
# brew 'libidl'
# brew 'libidn'
# brew 'libimobiledevice'
# brew 'libinfinity'
# brew 'libiptcdata'
# brew 'libkate'
# brew 'libkml'
# brew 'libksba'
# brew 'liblas'
# brew 'liblastfm'
# brew 'liblinear'
# brew 'liblo'
# brew 'liblockfile'
# brew 'liblqr'
# brew 'liblunar'
# brew 'libmagic'
# brew 'libmatroska'
# brew 'libmemcached'
# brew 'libmicrohttpd'
# brew 'libmikmod'
# brew 'libming'
# brew 'libmms'
# brew 'libmp3splt'
# brew 'libmpc'
# brew 'libmpd'
# brew 'libmpdclient'
# brew 'libmpeg2'
# brew 'libmtp'
# brew 'libmusicbrainz'
# brew 'libmxml'
# brew 'libnet'
# brew 'libnfc'
# brew 'libnids'
# brew 'libogg'
# brew 'liboil'
# brew 'libopennet'
# brew 'liboping'
# brew 'libosip'
# brew 'libotr'
# brew 'libpano'
# brew 'libpar2'
# brew 'libpcap'
# brew 'libplist'
# brew 'libpst'
# brew 'libpurple'
# brew 'libpuzzle'
# brew 'libqalculate'
# brew 'libqglviewer'
# brew 'libquicktime'
# brew 'librasterlite'
# brew 'libraw'
# brew 'libreplaygain'
# brew 'librets'
# brew 'librsvg'
# brew 'libsamplerate'
# brew 'libsgml'
# brew 'libshout'
# brew 'libsigc++'
# brew 'libsigsegv'
# brew 'libsmi'
# brew 'libsndfile'
# brew 'libspatialite'
# brew 'libspiro'
# brew 'libspotify'
# brew 'libssh'
# brew 'libssh2'
# brew 'libstfl'
# brew 'libstxxl'
# brew 'libsvg'
# brew 'libsvg-cairo'
# brew 'libsvm'
# brew 'libtasn1'
# brew 'libtecla'
# brew 'libtermkey'
# brew 'libtiff'
# brew 'libtommath'
# brew 'libtool'
# brew 'libtorrent'
# brew 'libtorrent-rasterbar'
# brew 'libtrace'
# brew 'libunique'
# brew 'libunistring'
# brew 'libupnp'
# brew 'libusb'
# brew 'libusb-compat'
# brew 'libutf'
# brew 'libvbucket'
# brew 'libvirt'
# brew 'libvo-aacenc'
# brew 'libvorbis'
# brew 'libvpx'
# brew 'libwbxml'
# brew 'libwmf'
# brew 'libwpd'
# brew 'libwpg'
# brew 'libwps'
# brew 'libxdiff'
# brew 'libxmi'
# brew 'libxml++'
# brew 'libxml2'
# brew 'libxmlsec1'
# brew 'libxslt'
# brew 'libxspf'
# brew 'libyaml'
# brew 'libyubikey'
# brew 'libzdb'
# brew 'libzip'
# brew 'libzzip'
# brew 'lifelines'
# brew 'lightning'
# brew 'lighttpd'
# brew 'lilypond'
# brew 'link-grammar'
# brew 'linklint'
# brew 'links'
# brew 'liquibase'
# brew 'litmus'
# brew 'little-cms'
# brew 'little-cms2'
# brew 'llvm'
# brew 'lmutil'
# brew 'lockrun'
# brew 'log4cplus'
# brew 'log4cpp'
# brew 'log4cxx'
# brew 'log4shib'
# brew 'logcheck'
# brew 'logentries'
# brew 'logrotate'
# brew 'logstalgia'
# brew 'logtalk'
# brew 'lolcode'
# brew 'lorem'
# brew 'loudmouth'
# brew 'lout'
# brew 'lpc21isp'
# brew 'lrzip'
# brew 'lrzsz'
# brew 'lsdvd'
# brew 'lsof'
# brew 'lua'
# brew 'luajit'
# brew 'luarocks'
# brew 'luciddb'
# brew 'lv'
# brew 'lxsplit'
# brew 'lynx'
# brew 'lysp'
# brew 'lzip'
# brew 'lzlib'
# brew 'lzo'
# brew 'lzop'
# brew 'm4'
# brew 'mac-robber'
# brew 'macvim'
# brew 'mad'
# brew 'madplay'
# brew 'mafft'
# brew 'magit'
# brew 'mailcheck'
# brew 'mairix'
# brew 'make'
# brew 'makeicns'
# brew 'makensis'
# brew 'malbolge'
# brew 'mame'
# brew 'man2html'
# brew 'mapnik'
# brew 'mapserver'
# brew 'mariadb'
# brew 'markdown'
# brew 'mathgl'
# brew 'mathomatic'
# brew 'maven-shell'
# brew 'mawk'
# brew 'maxima'
# brew 'mcabber'
# brew 'mcl'
# brew 'mcpp'
# brew 'mcrypt'
# brew 'md'
# brew 'md5deep'
# brew 'md5sha1sum'
# brew 'mdbtools'
# brew 'mdf2iso'
# brew 'mdxmini'
# brew 'mecab'
# brew 'mecab-ipadic'
# brew 'media-info'
# brew 'mediatomb'
# brew 'memcache-top'
# brew 'memcached'
# brew 'memcacheq'
# brew 'memtester'
# brew 'mercurial'
# brew 'mesalib-glw'
# brew 'mess'
# brew 'metalua'
# brew 'metapixel'
# brew 'metaproxy'
# brew 'metasploit'
# brew 'metis'
# brew 'mftrace'
# brew 'mg'
# brew 'mhash'
# brew 'midgard2'
# brew 'midnight-commander'
# brew 'mikmod'
# brew 'minbif'
# brew 'minc'
# brew 'minicom'
# brew 'minisat'
# brew 'minised'
# brew 'miniupnpc'
# brew 'minuit2'
# brew 'mira'
# brew 'mit-scheme'
# brew 'mjpegtools'
# brew 'mkclean'
# brew 'mkcue'
# brew 'mksh'
# brew 'mktorrent'
# brew 'mkvalidator'
# brew 'mkvtoolnix'
# brew 'mldonkey'
# brew 'mlton'
# brew 'mmv'
# brew 'mobile-shell'
# brew 'mod_python'
# brew 'mod_wsgi'
# brew 'mogenerator'
# brew 'monetdb'
# brew 'mongoose'
# brew 'mongrel2'
# brew 'monotone'
# brew 'montage'
# brew 'moreutils'
# brew 'mosh'
# brew 'mosml'
# brew 'mosquitto'
# brew 'movgrab'
# brew 'mp3cat'
# brew 'mp3check'
# brew 'mp3gain'
# brew 'mp3info'
# brew 'mp3splt'
# brew 'mp3val'
# brew 'mp3wrap'
# brew 'mp4v2'
# brew 'mpack'
# brew 'mpc'
# brew 'mpd'
# brew 'mpdas'
# brew 'mpdscribble'
# brew 'mpfr'
# brew 'mpg123'
# brew 'mpg321'
# brew 'mpgtx'
# brew 'mpich2'
# brew 'mpio'
# brew 'mplayer'
# brew 'mpop'
# brew 'mpsolve'
# brew 'mr'
# brew 'mrfast'
# brew 'mrtg'
# brew 'mscgen'
# brew 'msgpack'
# brew 'msgpack-rpc'
# brew 'msmtp'
# brew 'mt-daapd'
# brew 'mtools'
# brew 'mtr'
# brew 'mu'
# brew 'multimarkdown'
# brew 'multitail'
# brew 'muparser'
# brew 'mupdf'
# brew 'muscle'
# brew 'musepack'
# brew 'mydumper'
# brew 'mytop'
# brew 'n2n'
# brew 'nacl'
# brew 'nagios'
# brew 'nagios-plugins'
# brew 'nailgun'
# brew 'nano'
# brew 'narwhal'
# brew 'nasm'
# brew 'naturaldocs'
# brew 'nauty'
# brew 'ncdu'
# brew 'ncftp'
# brew 'ncmpc'
# brew 'ncmpcpp'
# brew 'ncrack'
# brew 'ncurses'
# brew 'ncview'
# brew 'ndiff'
# brew 'neko'
# brew 'neo4j'
# brew 'neon'
# brew 'nesc'
# brew 'net-nuclear'
# brew 'net-snmp'
# brew 'net6'
# brew 'netcat'
# brew 'netcdf'
# brew 'netpbm'
# brew 'netsed'
# brew 'nettle'
# brew 'newick-utils'
# brew 'newlisp'
# brew 'ngircd'
# brew 'ngrep'
# brew 'ngspice'
# brew 'nickle'
# brew 'nimrod'
# brew 'nkf'
# brew 'nload'
# brew 'nlopt'
# brew 'nmap'
# brew 'node'
# brew 'notmuch'
# brew 'noweb'
# brew 'nrg2iso'
# brew 'nrpe'
# brew 'nspr'
# brew 'nss'
# brew 'ntfs-3g'
# brew 'ntl'
# brew 'nu'
# brew 'num-utils'
# brew 'nuttcp'
# brew 'nvi'
# brew 'nylon'
# brew 'nzbget'
# brew 'o-make'
# brew 'oath-toolkit'
# brew 'obby'
# brew 'objective-caml'
# brew 'ocp'
# brew 'ocrad'
# brew 'octave'
# brew 'ode'
# brew 'odt2txt'
# brew 'offline-imap'
# brew 'oggz'
# brew 'ogmtools'
# brew 'ohcount'
# brew 'omega'
# brew 'oniguruma'
# brew 'oorexx'
# brew 'open-babel'
# brew 'open-cobol'
# brew 'open-mesh'
# brew 'open-mpi'
# brew 'open-ocd'
# brew 'open-scene-graph'
# brew 'open-sg'
# brew 'open-sp'
# brew 'open-vcdiff'
# brew 'opencc'
# brew 'opencolorio'
# brew 'openconnect'
# brew 'opencore-amr'
# brew 'opencv'
# brew 'openexr'
# brew 'openfst'
# brew 'openimageio'
# brew 'openjpeg'
# brew 'openldap'
# brew 'openmeeg'
# brew 'opensaml'
# brew 'openslp'
# brew 'opentracker'
# brew 'openttd'
# brew 'openvpn'
# brew 'ophcrack'
# brew 'optipng'
# brew 'opus'
# brew 'opus-tools'
# brew 'orbit'
# brew 'orc'
# brew 'orpie'
# brew 'ortp'
# brew 'osm-pbf'
# brew 'osm2pgsql'
# brew 'osmosis'
# brew 'osslsigncode'
# brew 'ossp-uuid'
# brew 'otx'
# brew 'owfs'
# brew 'p0f'
# brew 'p11-kit'
# brew 'p7zip'
# brew 'pam_yubico'
# brew 'paml'
# brew 'pango'
# brew 'pangomm'
# brew 'paperkey'
# brew 'par'
# brew 'par2'
# brew 'par2tbb'
# brew 'parallel'
# brew 'pari'
# brew 'parmetis'
# brew 'parrot'
# brew 'patchutils'
# brew 'pathfinder'
# brew 'pax-construct'
# brew 'pax-runner'
# brew 'pbc'
# brew 'pbc-sig'
# brew 'pbzip2'
# brew 'pcal'
# brew 'pcb'
# brew 'pdal'
# brew 'pdf2image'
# brew 'pdf2json'
# brew 'pdf2svg'
# brew 'pdfcrack'
# brew 'pdfgrep'
# brew 'pdfjam'
# brew 'pdflib-lite'
# brew 'pdftohtml'
# brew 'pdksh'
# brew 'pdnsd'
# brew 'pdsh'
# brew 'peg'
# brew 'peg-markdown'
# brew 'perceptualdiff'
# brew 'percona-server'
# brew 'percona-toolkit'
# brew 'perforce'
# brew 'perforce-proxy'
# brew 'perforce-server'
# brew 'perl'
# brew 'pg_top'
# brew 'pgbouncer'
# brew 'pgdbf'
# brew 'pgpool-ii'
# brew 'pgtap'
# brew 'phantomjs'
# brew 'phash'
# brew 'phoronix-test-suite'
# brew 'phyml'
# brew 'physfs'
# brew 'pianobar'
# brew 'picoc'
# brew 'picocom'
# brew 'pidof'
# brew 'pig'
# brew 'pigz'
# brew 'pil'
# brew 'pincaster'
# brew 'pinentry'
# brew 'pipebench'
# brew 'pipemeter'
# brew 'pit'
# brew 'pixie'
# brew 'pixman'
# brew 'pkg-config'
# brew 'play'
# brew 'playdar'
# brew 'plink'
# brew 'plod'
# brew 'plotutils'
# brew 'plowshare'
# brew 'plt-racket'
# brew 'plustache'
# brew 'plzip'
# brew 'pmdmini'
# brew 'pms'
# brew 'png2ico'
# brew 'pngcheck'
# brew 'pngcrush'
# brew 'pngnq'
# brew 'pngrewrite'
# brew 'poco'
# brew 'podofo'
# brew 'points2grid'
# brew 'polipo'
# brew 'polyml'
# brew 'poppler'
# brew 'popt'
# brew 'portaudio'
# brew 'portmidi'
# brew 'pos'
# brew 'poster'
# brew 'postgis'
# brew 'postgresql'
# brew 'postmark'
# brew 'potrace'
# brew 'pound'
# brew 'povray'
# brew 'pow'
# brew 'ppl'
# brew 'ppss'
# brew 'premake'
# brew 'primer3'
# brew 'primesieve'
# brew 'privoxy'
# brew 'proctools'
# brew 'prodigal'
# brew 'proguard'
# brew 'proj'
# brew 'proxytunnel'
# brew 'psftools'
# brew 'psgrep'
# brew 'pstoedit'
# brew 'pstree'
# brew 'pth'
# brew 'ptunnel'
# brew 'puf'
# brew 'pulledpork'
# brew 'pure'
# brew 'pure-ftpd'
# brew 'putmail'
# brew 'putmail-queue'
# brew 'putty'
# brew 'pv'
# brew 'pwgen'
# brew 'pwnat'
# brew 'pwsafe'
# brew 'py2cairo'
# brew 'pygobject'
# brew 'pygtk'
# brew 'pygtkglext'
# brew 'pypy'
# brew 'pyqt'
# brew 'pyqwt'
# brew 'pyside'
# brew 'pyside-tools'
# brew 'qca'
# brew 'qcachegrind'
# brew 'qd'
# brew 'qdbm'
# brew 'qemu'
# brew 'qfits'
# brew 'qhull'
# brew 'qi'
# brew 'qjson'
# brew 'qpdf'
# brew 'qprint'
# brew 'qrencode'
# brew 'qrupdate'
# brew 'qscintilla2'
# brew 'qstat'
# brew 'qt-mobility'
# brew 'quantlib'
# brew 'quassel'
# brew 'quex'
# brew 'quickfix'
# brew 'quicktree'
# brew 'quilt'
# brew 'quvi'
# brew 'qwt'
# brew 'qxmpp'
# brew 'radare2'
# brew 'ragel'
# brew 'rails-completion'
# brew 'rakudo-star'
# brew 'ranger'
# brew 'raptor'
# brew 'rarian'
# brew 'rasqal'
# brew 'rats'
# brew 'rbenv'
# brew 'rbenv-gemset'
# brew 'rbenv-vars'
# brew 'rc'
# brew 'rdesktop'
# brew 'rdiff-backup'
# brew 'rds-command-line-tools'
# brew 're2'
# brew 're2c'
# brew 'readline'
# brew 'readosm'
# brew 'readpst'
# brew 'reattach-to-user-namespace'
# brew 'rebar'
# brew 'recode'
# brew 'recutils'
# brew 'redis'
# brew 'redis-tools'
# brew 'redland'
# brew 'redo'
# brew 'redsocks'
# brew 'regina-rexx'
# brew 'remind'
# brew 'ren'
# brew 'rename'
# brew 'renameutils'
# brew 'repl'
# brew 'repo'
# brew 'reposurgeon'
# brew 'resty'
# brew 'rfcdiff'
# brew 'rfcmarkup'
# brew 'rfcstrip'
# brew 'rhino'
# brew 'riak'
# brew 'riak-search'
# brew 'riemann'
# brew 'rinetd'
# brew 'ringojs'
# brew 'ripmime'
# brew 'rlog'
# brew 'rlwrap'
# brew 'rmcast'
# brew 'rmtrash'
# brew 'rnv'
# brew 'robodoc'
# brew 'rock'
# brew 'rogue'
# brew 'rom-tools'
# brew 'roundup'
# brew 'rpg'
# brew 'rpl'
# brew 'rpm2cpio'
# brew 'rrdtool'
# brew 'rsense'
# brew 'rsnapshot'
# brew 'rsyslog'
# brew 'rt-audio'
# brew 'rtmpdump'
# brew 'rtorrent'
# brew 'rtpbreak'
# brew 'rubber'
# brew 'rubinius'
# brew 'ruby'
# brew 'ruby-build'
# brew 'ruby-enterprise-edition'
# brew 'ruby-odbc'
# brew 'runcocoa'
# brew 'runit'
# brew 'rush'
# brew 'rust'
# brew 'rxvt-unicode'
# brew 'rzip'
# brew 's-lang'
# brew 's3-backer'
# brew 's3cmd'
# brew 's3fs'
# brew 's3sync'
# brew 'saga-core'
# brew 'salt'
# brew 'sam2p'
# brew 'samba'
# brew 'samtools'
# brew 'sane-backends'
# brew 'sary'
# brew 'savana'
# brew 'saxon'
# brew 'saxon-b'
# brew 'sbcl'
# brew 'sbt'
# brew 'sc68'
# brew 'scalate'
# brew 'scalpel'
# brew 'scamperema'
# brew 'scantailor'
# brew 'scheme48'
# brew 'schroedinger'
# brew 'scm-manager'
# brew 'scons'
# brew 'scotch'
# brew 'screen'
# brew 'scrollkeeper'
# brew 'scrotwm'
# brew 'scrub'
# brew 'scrypt'
# brew 'scsh'
# brew 'scummvm'
# brew 'sdcc'
# brew 'sdelta3'
# brew 'sdf'
# brew 'sdl'
# brew 'sdl_gfx'
# brew 'sdl_image'
# brew 'sdl_mixer'
# brew 'sdl_net'
# brew 'sdl_rtf'
# brew 'sdl_sound'
# brew 'sdl_ttf'
# brew 'sedna'
# brew 'selenium-server-standalone'
# brew 'ser2net'
# brew 'serf'
# brew 'sersniff'
# brew 'sgrep'
# brew 'shakespeare'
# brew 'shapelib'
# brew 'shaper-probe'
# brew 'shared-mime-info'
# brew 'shark'
# brew 'shell.fm'
# brew 'shen'
# brew 'shiboken'
# brew 'shmux'
# brew 'shntool'
# brew 'shocco'
# brew 'shorten'
# brew 'shtool'
# brew 'sic'
# brew 'sickbeard'
# brew 'sigar'
# brew 'signing-party'
# brew 'silk'
# brew 'simgrid'
# brew 'simh'
# brew 'since'
# brew 'sip'
# brew 'sipcalc'
# brew 'sipp'
# brew 'sipsak'
# brew 'sisc-scheme'
# brew 'sispmctl'
# brew 'sitecopy'
# brew 'ski'
# brew 'skipfish'
# brew 'skktools'
# brew 'skytools'
# brew 'sl'
# brew 'sleepwatcher'
# brew 'sleuthkit'
# brew 'sloccount'
# brew 'slrn'
# brew 'smake'
# brew 'smartmontools'
# brew 'smartypants'
# brew 'smlnj'
# brew 'smpeg'
# brew 'snappy'
# brew 'snobol4'
# brew 'snort'
# brew 'sntop'
# brew 'socat'
# brew 'sofia-sip'
# brew 'solid'
# brew 'solr'
# brew 'sonar'
# brew 'sound-touch'
# brew 'source-highlight'
# brew 'sox'
# brew 'spark'
# brew 'spatialindex'
# brew 'spatialite-tools'
# brew 'spawn-fcgi'
# brew 'speex'
# brew 'sphinx'
# brew 'spidermonkey'
# brew 'spim'
# brew 'spin'
# brew 'spiped'
# brew 'splint'
# brew 'spring-roo'
# brew 'sproxy'
# brew 'sqsh'
# brew 'squashfs'
# brew 'squid'
# brew 'squirrel'
# brew 'srecord'
# brew 'ssdeep'
# brew 'ssed'
# brew 'ssh-copy-id'
# brew 'sshfs'
# brew 'sshguard'
# brew 'sshuttle'
# brew 'ssldump'
# brew 'sslscan'
# brew 'ssss'
# brew 'stanford-parser'
# brew 'star'
# brew 'staticrouted'
# brew 'stgit'
# brew 'stklos'
# brew 'storm'
# brew 'stormfs'
# brew 'stow'
# brew 'stp'
# brew 'strategoxt'
# brew 'streamripper'
# brew 'stress'
# brew 'stunnel'
# brew 'style-check'
# brew 'sub2srt'
# brew 'subversion'
# brew 'suite-sparse'
# brew 'sundials'
# brew 'surfraw'
# brew 'svdlibc'
# brew 'svg2pdf'
# brew 'svg2png'
# brew 'swaks'
# brew 'swfmill'
# brew 'swftools'
# brew 'swi-prolog'
# brew 'swig'
# brew 'swish-e'
# brew 'syck'
# brew 'symphony'
# brew 'synergy'
# brew 'synfig'
# brew 'synfigstudio'
# brew 'syslog-ng'
# brew 'szip'
# brew 'szl'
# brew 't1utils'
# brew 'ta-lib'
# brew 'tabbed'
# brew 'tabix'
# brew 'taglib'
# brew 'tal'
# brew 'talk-filters'
# brew 'talloc'
# brew 'tarsnap'
# brew 'task'
# brew 'tbb'
# brew 'tcl'
# brew 'tclap'
# brew 'tcpdump'
# brew 'tcpflow'
# brew 'tcping'
# brew 'tcpreplay'
# brew 'tcpstat'
# brew 'tcptrace'
# brew 'tcptraceroute'
# brew 'tcptrack'
# brew 'tcpurify'
# brew 'teapot'
# brew 'teem'
# brew 'term'
# brew 'tesseract'
# brew 'testdisk'
# brew 'tetgen'
# brew 'texinfo'
# brew 'thc-pptp-bruter'
# brew 'the_silver_searcher'
# brew 'theora'
# brew 'thrift'
# brew 'thrulay'
# brew 'tidy'
# brew 'tidyp'
# brew 'tiff2png'
# brew 'tig'
# brew 'tiger-vnc'
# brew 'timbl'
# brew 'timedog'
# brew 'tin'
# brew 'tinc'
# brew 'tintin'
# brew 'tiny-fugue'
# brew 'tinyproxy'
# brew 'tinysvm'
# brew 'titlecase'
# brew 'tivodecode'
# brew 'tk'
# brew 'tkdiff'
# brew 'tmap'
# brew 'tmpreaper'
# brew 'tmux'
# brew 'tn5250'
# brew 'tnef'
# brew 'todo-txt'
# brew 'tofrodos'
# brew 'toilet'
# brew 'tokyo-cabinet'
# brew 'tokyo-dystopia'
# brew 'tokyo-tyrant'
# brew 'tomcat'
# brew 'topgit'
# brew 'tophat'
# brew 'tor'
# brew 'torsocks'
# brew 'trafficserver'
# brew 'trafshow'
# brew 'trang'
# brew 'transcode'
# brew 'transmission'
# brew 'tre'
# brew 'tree'
# brew 'treecc'
# brew 'treeline'
# brew 'triangle'
# brew 'tsung'
# brew 'ttf2eot'
# brew 'ttf2pt1'
# brew 'tth'
# brew 'ttyrec'
# brew 'ttytter'
# brew 'tup'
# brew 'two-lame'
# brew 'txt2man'
# brew 'txt2tags'
# brew 'typespeed'
# brew 'uade'
# brew 'uchardet'
# brew 'ucl'
# brew 'udis86'
# brew 'udns'
# brew 'udunits'
# brew 'ufraw'
# brew 'uif2iso'
# brew 'uim'
# brew 'unafold'
# brew 'unbound'
# brew 'uncrustify'
# brew 'unfs3'
# brew 'ungif'
# brew 'unifdef'
# brew 'unison'
# brew 'unittest'
# brew 'unixodbc'
# brew 'unp'
# brew 'unpaper'
# brew 'unrtf'
# brew 'unshield'
# brew 'unyaffs'
# brew 'uptimed'
# brew 'upx'
# brew 'uriparser'
# brew 'urlview'
# brew 'urweb'
# brew 'usbmuxd'
# brew 'ushare'
# brew 'utimer'
# brew 'uudeview'
# brew 'uwsgi'
# brew 'v8'
# brew 'v8cgi'
# brew 'vala'
# brew 'valkyrie'
# brew 'vbindiff'
# brew 'vcdimager'
# brew 'vcftools'
# brew 'vcodex'
# brew 'vcprompt'
# brew 'vde'
# brew 'velvet'
# brew 'verilator'
# brew 'vf'
# brew 'vgmstream'
# brew 'vice'
# brew 'vifm'
# brew 'vilistextum'
# brew 'vimeo-downloader'
# brew 'vimpager'
# brew 'vimpc'
# brew 'vip'
# brew 'vips'
# brew 'virtualhost.sh'
# brew 'virtuoso'
# brew 'visitors'
# brew 'visualnetkit'
# brew 'vmalloc'
# brew 'vnstat'
# brew 'vobcopy'
# brew 'voldemort'
# brew 'vorbis-tools'
# brew 'vorbisgain'
# brew 'vpnc'
# brew 'vrpn'
# brew 'vsftpd'
# brew 'vte'
# brew 'vtk'
# brew 'w3m'
# brew 'wait_on'
# brew 'wakeonlan'
# brew 'watch'
# brew 'wavpack'
# brew 'wbox'
# brew 'wdfs'
# brew 'wdiff'
# brew 'web100clt'
# brew 'webalizer'
# brew 'webfs'
# brew 'webkit2png'
# brew 'webp'
# brew 'weechat'
# brew 'wemux'
# brew 'whatmask'
# brew 'when'
# brew 'whirr'
# brew 'whohas'
# brew 'wiggle'
# brew 'willgit'
# brew 'wine'
# brew 'winetricks'
# brew 'winexe'
# brew 'wkhtmltopdf'
# brew 'wla-dx'
# brew 'wmctrl'
# brew 'wol'
# brew 'wopr'
# brew 'wordnet'
# brew 'wp-cli'
# brew 'wps2odt'
# brew 'wput'
# brew 'wrangler'
# brew 'writerperfect'
# brew 'wrk'
# brew 'wtf'
# brew 'wv'
# brew 'wv2'
# brew 'wwwoffle'
# brew 'wxmac'
# brew 'wyrd'
# brew 'x264'
# brew 'x3270'
# brew 'xa'
# brew 'xapian'
# brew 'xar'
# brew 'xaric'
# brew 'xastir'
# brew 'xaw3d'
# brew 'xchat'
# brew 'xclip'
# brew 'xdelta'
# brew 'xdotool'
# brew 'xerces-c'
# brew 'xml-coreutils'
# brew 'xml-security-c'
# brew 'xml-tooling-c'
# brew 'xml2rfc'
# brew 'xmlformat'
# brew 'xmlrpc-c'
# brew 'xmlto'
# brew 'xmltoman'
# brew 'xmoto'
# brew 'xmp'
# brew 'xpa'
# brew 'xpdf'
# brew 'xplanet'
# brew 'xqilla'
# brew 'xrootd'
# brew 'xspin'
# brew 'xspringies'
# brew 'xsw'
# brew 'xvid'
# brew 'xz'
# brew 'yaf'
# brew 'yajl'
# brew 'yamdi'
# brew 'yaml-cpp'
# brew 'yara'
# brew 'yarp'
# brew 'yasm'
# brew 'yaws'
# brew 'yaz'
# brew 'yazpp'
# brew 'yconalyzer'
# brew 'yeti'
# brew 'ykclient'
# brew 'ykpers'
# brew 'youtube-dl'
# brew 'yuicompressor'
# brew 'yydecode'
# brew 'z'
# brew 'zbar'
# brew 'zdelta'
# brew 'zebra'
# brew 'zeromq'
# brew 'zile'
# brew 'zint'
# brew 'zlib'
# brew 'znc'
# brew 'zookeeper'
# brew 'zsh'
# brew 'zsh-completions'
# brew 'zsh-lovers'
# brew 'zssh'
# brew 'zsync'
# brew 'zzuf'

##
# brew-install-our-base-packages-manually.sh
#
# Use Homebrew to install our favorite typical-user packages
# that may need to be installed manually because of passwords,
# or moving files, or more-complex issues that need a human.
##

## Environment-related

# DisplayLink enables adding monitors
cask 'displaylink'

# Java language for running many applications
cask 'java'

# Karabiner remaps keyboard keys
cask 'karabiner'

## Media-related

# Adobe Air player for multimedia content
cask 'adobe-air'

# Adobe Reader for PDF files
cask 'adobe-reader'


## Misc

cask 'flip4mac'
cask 'google-hangouts'
cask 'inky'
cask 'node'
cask 'obs'
cask 'pandoc'
cask 'prey'
cask 'seil'
cask 'teamviewer'
cask 'unity-web-player'
cask 'unity3d'
cask 'zoomus'


## Mac App Store

mas 'Numbers', id: 409203825
mas 'Pages', id: 409201541
mas 'Slack', id: 803453959
mas 'Sip', id: 507257563
mas 'Simplenote', id: 692867256
mas 'Todoist', id: 585829637

##
# brew-install-our-stacks-automatically.sh
#
# Use Homebrew to install our favorite tech-related packages
# that can be installed fully automatically i.e. unattended;
# these packages do not ask for passwords, do not have any
# prompts, and do not have any issues that need a human.
#
# If you're using this file and you find any packages that
# do not install automatically, please let us know by opening
# an issue, or emailing us, or creating a pull request. Thanks!
#
# ## Link
#
# Some of the brew packages need to link to others.
#
#   * `brew link cmake` before mysql
#   * `brew link cmake` before wireshark can be installed
#   * `brew link cmake` before homebrew/science/opencv
#   * `brew link pandoc` before shellcheck can be installed
#
##

##
# System
##

# XQuartz provides X.Org X Window System that runs on OS X.
cask 'xquartz'

##
# Environment
##

# Code Climate Platform for all static analysic
brew tap codeclimate/formulas && brew 'codeclimate'

##
# Shell
##

# GUI for rsync
brew 'grsync'

# Shell script syntax check linter
brew link pandoc; brew 'shellcheck'

# BATS: Bash Automated Testing System
cask 'bats'

##
# Clients
##

# Shuttle: simple SSH shortcut menu
cask 'shuttle'

# Fugu: a graphical shell for SSH and FTP.
cask 'fugu'

# Charles: enables a developer to view HTTP traffic.
cask 'charles'


##
# Languages
##

# Apache Maven is a software project management and comprehension tool.
brew 'maven'

# Apache Spark is for analytics
brew 'apache-spark'
  
  
##
# Mac programming
##

# Dash documentation browser and code snippet manager
cask 'dash'

# Realm browser for the Realm embedded database
cask 'realm-browser'

# Tunnelblick remote access VPN
cask 'tunnelblick'

##
# Networking
##

# Wireshark network monitoring, with the QT GUI.
brew link cmake; cask 'wireshark --with-qt'

# Wireshark-chmodbft enables regular users to capture network packets.
cask 'wireshark-chmodbpf'

# Charles web debugging proxy
cask 'charles'

# Siege is an http load testing and benchmarking utility.
brew 'siege'

##
# Virtual environments
##

# Docker assembles applications from components.
cask 'docker'

# Vagrant creates and configures portable development environments.
cask 'vagrant'
cask 'vagrant-manager'

# VirtualBox creates and configures portable development environments, by Oracle.
cask 'virtualbox'

# Terraform common configuration to launch infrastructure.
brew 'terraform'

# corectl provides CoreOS over macOS made very simple
cask 'corectl'

# Kubernetes Solo cluster for macOS
cask 'kube-solo'

##
# IDE
##

# Eclipse is a large programming IDE built on Java
cask 'eclipse-ide'
cask 'eclipse-platform'

##
# Databases
#
# This section installs many databases and database tooling:
# Cassandra, CouchDB, Hadoop, MariaDB, MongoDB, PostgreSQL,
# RabbitMQ, Redis, Riak, Sphinx, SQLite. Notably *not* MySQL.
##

# Cassandra database.
brew 'cassandra'

# CouchDB database, esp. for document-oriented storage.
brew 'couchdb'

# Hadoop database.
brew 'hadoop'

# MariaDB database; prefer this over MySQL.
brew 'mariadb'

# MongoDB database.
brew 'mongodb'

# PostgreSQL database.
brew 'postgres'

# PostgreSQL database.
brew 'postgresql'

# Postgres App provides a Mac-friendly database.
cask 'postgres'

# Prisma replaces traditional ORMs and adds GraphQL
tap 'prisma/prisma'
brew 'prisma'

# Postgres admin GUI
brew 'pgadmin3'

# RabbitMQ enterprise message queue based on the emerging AMQP standard.
brew 'rabbitmq'

# Redis database, esp. for key-value cache and store, and data structures.
brew 'redis'

# Riak open-source distributed database.
brew 'riak'

# SQLite database: self-contained, serverless, zero-configuration, transactional engine.
brew 'sqlite && brew link sqlite'

# ZeroMQ message queue
brew 'zeromq'

##
# Database searchers
#
# TODO: add more here
##

# Sphinx search engine.
brew link cmake; brew 'mysql; brew install postgresql; brew install sphinx'

##
# Database managers
#
# TODO: add pgadmin etc.
##

# MySQL Workbench database editor.
brew link cmake; cask 'mysqlworkbench'

# Realm browser mobile database editor.
cask 'realm-browser'

# Sequel Pro database management application.
cask 'sequel-pro'

# Toad database manager by Dell.
cask 'toad'

# Valentina Studio database manager.
cask 'valentina-studio'

##
# Data analytics
##

# Elasticsearch is a real-time, distributed storage, search, and analytics engine.
brew 'elasticsearch'

# Logstash helps parse, enrich, transform, and buffer data from a variety of sources.
brew 'logstash'

# Kibana is an open source analytics and visualization platform designed to work with Elasticsearch. 
brew 'kibana'

##
# Markup languages
#
# For example this section is a good place for HTML tools,
# Markdown tools, UML tools, XML tools, and similar.
##

# Pandoc converts among various formats, such as Markdown and HTML
brew 'pandoc'

## Markdown

# MacDown simple markdown editor
cask 'macdown'

## UML

# StarUML modeling tool
cask 'staruml'

# PlantUML markup text to diagram
brew 'plantuml'

## XML

# XML converter
brew 'xmlstarlet'

# Libxml2 is the XML C parser and toolkit.
brew 'libxml2'

# Libxslt is the XSLT C library for the XML EXtensible Stylesheet Language.
brew 'libxslt'

##
# Programming languages
#
# This section installs many programming languages:
# Clojure, Elixir, Erlang, Go, Haskell, Java, JavaScript,
# Perl, Python, R, Ruby, Scala, Swift, and tooling.
##

## Clojure

# Clojure programming language compiler.
brew 'clojure-compiler'

# Leiningen automates Clojure projects.
brew 'leiningen'

## Elixir

# Elixir programming language built on top of the Erlang VM.
brew 'elixir'

## Erlang

# Erlang programming language for scalable high-availability systems.
brew 'erlang'

## Go

# Go programming language by Google; compare `C`.
brew 'go'

## Haskell

# Cabal is a package manager for Haskell
brew 'ghc'
brew 'cabal-install'

## Java

# Java programming language
cask 'java'

# Gradle is a Java build tool
brew 'gradle'

# Maven is a Java build tool
brew 'maven'

# Spring Tool Suite is an Eclipse IDE for developing apps
cask 'sts'

# Jetty provides a Java web server and javax.servlet container
brew 'jetty'

# Apache Tomcat implements Java Servlet and JavaServer Pages technologies.
brew 'tomcat'

# Glassfish application server.
brew 'glassfish'

## JavaScript

# Node.js is a JavaScript platform for building fast, scalable network app.
brew 'node'

# PhantomJS is a headless WebKit scriptable with a JavaScript API.
brew 'phantomjs'

# V8 JavaScript Engine.
brew 'v8'

# JSON output using the shell
brew 'jo'

# JID JSON explorer
brew tap simeji/jid && brew 'jid'

## Perl

# Perl programming language, esp. for systems administration.
brew 'perl'

# Perl-Compatible Regular Expressions pattern matching tools.
brew 'pcre'

# CPAN search for perl modules
brew 'cpansearch'

## Python

# Python programming language, esp. for systems scripting.
brew 'python'
brew 'python3'

## R

# R programming language, esp. for statistics.
brew 'r'

## Ruby

# chruby changes the current Ruby.
brew 'chruby'

# JRuby is a high performance, stable, fully threaded Java implementation of Ruby.
brew 'jruby'

# Ruby programming language; compare `perl`, `python`.
brew 'ruby'

# Tool to install various implementations of Ruby.
brew 'ruby-install'

## Rust

# Rust programming language
brew 'rust'

## Scala

# Scala programming language, that runs on top of the JVM.
brew 'scala'

## iOS, Objective-C, Swift

# Alcatraz Xcode plugin manager
cask 'alcatraz'

# Appium test automation framework
cask 'appium'

# Carthage Xcode project dependency manager.
brew 'carthage'

# Command-line application launcher for the iOS Simulator
brew 'ios-sim'

# Tool to help with Swift style and conventions.
brew 'swiftlint'

# SourceKitten attaches to SourceKit AST.
brew 'sourcekitten'

# Taylor is a Swift code quality metrics tool.
brew 'taylor'

# Testflight Apple iOS testing service
cask 'testflight'

##
# Platforms
##

# Amazon Web Services (AWS) Command Line Interface (CLI)
brew install awscli

# AWS command line tools
brew tap wallix/awless
brew 'awless'

# Heroku app hosting
brew install heroku

##
# Art editors
##

# Xquarts
cask 'xquartz'

# Tap GUI
brew tap homebrew/gui

# Gimp pixel-based image editor, similar to Adobe Photoshop
cask 'gimp'

# Inkscape vector-based image  editor, similar to Adobe Illustrator
cask 'inkscape'

# Shotcut movie editor
cask 'shotcut'

# Image optimizer
cask 'imageoptim'

# Freemind mind map editor
cask 'freemind'

##
# Paid software
#
# This section installs the tools, which are free trial versions.
# We pay for licenses for all these for all our teammates.
#
# You may want to customize this section by deleting any items that
# you don't want to use or purchase, because this will save disk space.
##

## Paw.cloud

# Paw HTTP API testing tool
cask 'paw'

##
# Libraries
#
# We do this near the end of this file,
# because we expect these will already be
# installed by a bunch of the software above.
#
# This section here is really just to cover our
# bases to make sure we have the libraries that we
# sometimes need for building other software later on.
##

# THe libevent API provides provides asynchronous event notification and callbacks.
brew 'libevent'

# Magic number recognition library for file types.
brew 'libmagic'

# Audio/Visual converters
brew 'libav'

# Curl web fetcher
brew 'libcurl'

# Foreign Function Interface Library
brew 'libffi'

# Text encoding
brew 'libiconv'

# File magic number recognizer
brew 'libmagic'

# ncurses console nagivation
brew 'libncurses'

# Sodium secure cryptography
brew 'libsodium'

# Readline terminal input
brew 'libreadline'

# GNU libtool is a generic library support script.
brew 'libtool'

# XML handlers
brew 'libxml2'
brew 'libxslt'

# High-level interface to X.509 and CMS (Cryptographic Message Syntax)
brew 'libksba'

# V8 JavaScript
brew 'libv8'

# YAML markup language
brew 'libyaml'

# YAML lint validator
brew 'yamllint'

# ZIP file compression
brew 'libzip'

# Images
brew 'libjpg'
brew 'libpng'
brew 'libtiff'
brew 'libwebp'

##
# brew-install-our-tech-packages-manually.sh
#
# Use Homebrew to install our favorite tech-related packages
# that may need to be installed manually because of passwords,
# or moving files, or more-complex issues that need a human.
#
##

# Update - this is always the first step
brew update

# Emacs editor.
sudo rm /usr/bin/emacs &&
sudo rm -rf /usr/share/emacs &&
brew 'emacs --cocoa --srgb --use-git-head --HEAD &&'
ls -1 /usr/local/Cellar/emacs/*/bin/emacs |
tail -1 |
xargs -I{} sudo ln -sf "{}" /usr/bin/emacs

## Networking

# nmap network mapper is a security scanner
cask 'nmap'

# Wireshark network protocol analyzer
cask 'wireshark'

# Certbot: automatically enable HTTPS on your website via Let's Encrypt
brew 'certbot'

## Programming

# Netbeans Java IDE
cask 'netbeans'

# R statistics programming language
cask 'r'

## Deployments

# Vagrant lightweight, reproducible, portable development environments
cask 'vagrant'

# Heroku hosting utilities
cask 'heroku-toolbelt'

## Testing

# Selenium standalone server
brew 'selenium-server-standalone'

# Selenium webdriver for Chrome browser
brew 'chromedriver'

# Selenimum webdriver for Firefox browser
brew 'geckodriver'


########################### TODO ############################################

## Utility-Related

# Alfred: boost your efficiency with hotkeys, keywords, text expansion, etc.
brew 'alfred'

## Serializers

# Protocol buffers for serializing structured data; compare thrift.
brew 'protobuf'
brew 'protobuf-c'

# Thrift network serialization protocol; compare protobuf.
brew 'thrift'

## Tools

# Ansible is a simple way to automate apps and IT infrastructure.
brew 'ansible'
