# Setting up a Window Machine for Work
---

## Current Machine Specification

**HP Envy x360 13 Laptop**
- Ryzen 4500U APU
- 8 GB RAM
- 256 GB Storage (_I split my partition, totally unnecessary_)
  1. 175 GB Partition for Windows
  2. 81 GB Empty Partition ... _hoping to get ChromeOS here_
- Windows 10 OS - Home Edition

## Requirements

1. A laptop
2. A USB Drive (Preferably 8GB+) and hopefully your laptop supports the interface
3. Internet Connection
4. Your **time**.

## Reason For This Guide

This machine was really well priced the for the hardware included. I have been using a MacBook Pro since 2010 as a daily driver for my laptop use, and I found that a lot of the benefits of using the macOS is **missing** with a Windows Machine.

This is not a complete guide / reproduction of the macOS productivity; however, it will be continuously updated as I find better alternatives to quirks that I find with the Windows OS.

PS. **_The apple trackpad is heavily missed._**

## Step 1: Reinstall Windows OS

_There was a lot of crap installed with odd settings when I first booted up my computer._

**WARNING**: This step will remove all data from your main drive.

Go to: [Windows 10 Installation USB Drive Tool](https://www.microsoft.com/en-gb/software-download/windows10)

Have your laptop charging as you go through this process. Don't let it die during this.

#### Steps

1. Plug-in your USB Drive
2. Make sure your USB Drive is working
3. Download the Windows 10 installation tool to help you create your boot drive/Windows 10 installer
4. Run the tool, and create your Bootable USB Drive
5. After your USB drive is complete, we will now boot into it.
 - To simply boot from your USB drive from Windows 10 first click ```Windows Button``` > ```Power Icon```: This will show you your shutdown options.
 - While holding the ```shift``` key down, click ```restart``` from your shutdown options.
 - Your computer should shutdown and show you an advanced start up options
 - Select: ```Use a Device``` option.
 - Select your desired USB drive to boot from to start the reinstallation process.
6. By now, the Windows 10 installation process should start as the computer boots into the USB drive. At this moment: choose your language settings, enter in product keys if prompted along with Windows 10 versions, and then we go to: ```custom installation```. We are not _upgrading_ we are doing full reinstall.
7. We want to do a custom installation because the producing company probably split up your hard drives into different partitions, and we as tech savvy geniuses don't need such setup.
  - At this point, I would ```delete all the partitions```
  - You should have ```unallocated space``` with whatever size of hard drive you have (_it should be similar to the max size of the intended hard drive size!_)
  - Click ```next``` to let Windows to do its installation.
8. 99% of the time everything should be okay, and you will be on your way to setting up: ```Regions, Keyboard Layout, Account creation and etc```

**Now you are done reinstalling Windows 10.**

Even with running a dedicated uninstaller for most of the _bloatware_, Microsoft Windows Update continuously re-added some applications back, and HP provided some weird applications installed already.

It seems that when applications are installed in Windows, they leave a lot of hidden files, temporary files, and/or registry stuff throughout the computer; therefore, I found myself feeling better with a clean reinstall of the Windows OS.

```
**Note:** Depending on the model/make/producing company, some features of your laptop may behave differently -or- misbehave.

For example: My HP Envy required me to install: HP Command Center to control its fan speeds due to its horrendous bios software.
```

## Step 2: Update Windows 10

This step will save you the hassle of dealing with more headaches later, it is also one of the most annoying parts because it can take a while. So, I recommend that you are watching Netflix as you are sitting by your laptop as it updates.

#### Steps
1. ```Windows Key``` > ```Settings Icon``` > ```Updates & Security```
2. ```Windows Update``` > ```Check for Updates```
3. At this point, it should be downloading and installing bunch of updates. Some updates will say ```pending restart```, so when it seems that all the update listed are done downloading and installing and has the restart message, let the laptop restart by clicking ```restart now```
4. Let your laptop restart and go through the update process.

More reading for installing Windows can be read [here](https://www.reddit.com/r/pcmasterrace/comments/77pjvf/the_correct_way_to_install_windows_10/).

## Step 3: Browser of Choice

I am not going to judge for what browser you use, but if you intend to not use Microsoft Edge, I would install your go to browser now.

I personally have this setup:
- [Chrome](https://www.google.com/chrome/) > logged-in for personal account.
- [Firefox](https://www.mozilla.org/en-CA/firefox/new/) > logged-in with my work account.

This way, I don't need the hassle of switching profiles on chrome. I just open up Firefox when I'm working while I open up Chrome when I am not working.

## Step 4: Ninite, installing your main software

[Ninite](https://ninite.com/) allows you to create a single installer program for a customize group of applications that you want.

This is totally optional because you can download and install your applications one-by-one **or** if you want to specify where to install to.

My current application list from Ninite:
- Foxit Reader
- Revo Uninstaller **A must have in my opinion**
- WinDirStat
- Discord
- VLC
- Spotify
- 7-Zip
- Your Online Cloud Service (One Drive, Google Backup and Sync, Dropbox)

_I left out Steam because this should be your **working machine**._

## Step 5: Remove Preinstalled Applications

If you have Revo Uninstaller, this should be your go to uninstaller rather than the Windows' Uninstaller tool. Revo will help you remove these programs much nicer.

Revo Uninstaller has a tab called ```Windows App```. I would go through this list and start removing the apps that you don't need. If you are unsure what the app does, you can always Google it.

## Step 6: Windows Settings

From here on, you have a really good base point of a working machine. Therefore, every step from here will be **optional**.

Windows Settings to look at:
- ```Cortana:``` I don't choose to use it, but the choice is yours
- ```Privacy:``` Opt-out of whatever you are not comfortable with
- ```Personalization:``` Style your computer the way you like it

## Step 7: UELI App Launcher

Coming from macOS I really wanted a spotlight and Alfred alternative that is not the built-in Windows Search. There are a lot of different options, but I decided to go with UELI.

Instead of fumbling through folders, start menu, or even filling up your desktop, you can use a keyboard based application launcher to help you open your things.

[Check out UELI Here.](https://ueli.app/#/)

## Programming & Developing Setup

#### a) Visual Studio Code

A great integrated development environment. Really useful for your development needs. It will be useful for the other setup coming up as well.

You can get it [here](https://code.visualstudio.com).

#### b) Windows Subsystem for Linux (WSL)

Most likely when you are programming or developing a project, you will require some sort of a Linux environment.

Here are two great tutorials to help you set it up. I would flip back and forth with the two tutorials to set it up.
- [Firebase.io Tutorial](https://fireship.io/lessons/windows-10-for-web-dev/)
- [Microsoft Tutorial](https://docs.microsoft.com/en-us/windows/wsl/install-win10)

```Please Note: Installing the Windows Terminal App is heavily recommended```

#### c) Get a Text Editor for Windows

Notepad is great minimalist application, but at some point you may want a stronger editor.

Here are some that I recommend:
- Notepad++
- Sublime Text 2/3
- Atom.io

```
As of 06/20/2020, this is my current setup. I do have jupyterlab and python3 installed since I mainly program in Python.
```
