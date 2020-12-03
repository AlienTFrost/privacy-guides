<!--
Title: How to clean uninstall macOS apps using AppCleaner open source alternative
Description: Learn how to clean uninstall macOS apps using AppCleaner open source alternative.
Author: Sun Knudsen <https://github.com/sunknudsen>
Contributors: Sun Knudsen <https://github.com/sunknudsen>
Reviewers:
Publication date: 2020-09-21T15:50:15.415Z
Listed: true
-->

# How to clean uninstall macOS apps using AppCleaner open source alternative

[![How to clean uninstall macOS apps using AppCleaner open source alternative - YouTube](how-to-clean-uninstall-macos-apps-using-appcleaner-open-source-alternative.png)](https://www.youtube.com/watch?v=0nVOB0EE5ps "How to clean uninstall macOS apps using AppCleaner open source alternative - YouTube")

## Guide

### Step 1: create `/usr/local/bin` folder

```shell
sudo mkdir -p /usr/local/bin
sudo chown $USER:admin /usr/local/bin
```

### Step 2: download [app-cleaner.sh](app-cleaner.sh) ([PGP signature](./app-cleaner.sh.sig), [PGP public key](https://sunknudsen.com/sunknudsen.asc))

```shell
curl -o /usr/local/bin/app-cleaner.sh https://sunknudsen.com/static/media/privacy-guides/how-to-clean-uninstall-macos-apps-using-appcleaner-open-source-alternative/app-cleaner.sh
chmod +x /usr/local/bin/app-cleaner.sh
```

👍

---

## Usage

```console
$ app-cleaner.sh /Applications/AppCleaner.app
Checking for running processes...
Finding application data...
/Applications/AppCleaner.app
/Users/johndoe/Library/Preferences/net.freemacsoft.AppCleaner.plist
/Users/johndoe/Library/Saved Application State/net.freemacsoft.AppCleaner.savedState
Move application data to trash (y or n)? y
Moving application data to trash...
Done
```
