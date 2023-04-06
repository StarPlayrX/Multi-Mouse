# 🐭👾🖲️ Virtual Multi-Mouse 1.1.0 🖲️👾🐭

The best auto-config solution on the planets. Combines your spinner, trackball, mouse into a virtual multi-mouse! Written from the ground up with intelligent code. Designed for Batocera Linux for use with Emulation Station and RetroArch.

## 🐭👾🖲️ Get Ready Player One!

Virtual Multi-Mouse auto configures trackball, spinner, mouse into one virtual device. Multi-Mouse works with Batocera v35 or later. Recently tested on v35, v36 and v37. Official lightgun support is coming soon! Future versions may learn what types of games you playing and setup your relative and absolute might accordingly. In other words, VMM will start to learn.

Like Batocera, Virtual Multi-Mouse is made to just play! Need to change your mouse configuration? Within a flash VMM sets up the virtual mouse accordingly. All you need to do is reboot and run a game! The software automatically determines the proper mouse config for player 1 games.

Virtual Multi-Mouse uses sophisticated central intelligance gathering. VMM is programmed to be smart, very smart. Upon every fresh reboot, it does an awesome job reconfiguring all your mouse devices into one global mouse for player one. This software aims to be a zero-config-solution. We want VMM to be Auto-Magic!

Troubleshooting: If things are not working, try exiting your game and relaunching it. Sometimes VMM needs a jump start. If your mouse controllers are still not working, simply reboot Batocera. Still having trouble? Feel free to post an issue. This is getting more rare as VMM can anticipate problems.

At install, the Batocera.conf file is backed up. This is safegard incase something happens. Virtual Multi-Mouse sets the global index here for EmulationStation and RetroArch to configure and if for any reason that becomes defunct, your games could stop working. This is even more rare now but having a backup of this file with every install gives you peace of mind.

Virtual Multi-Mouse natively supports relative usb devices this includes mouse, trackballs and spinners. We currently do not support absolute devices which are multi-touch trackpads, lightguns and touch screens. These are absolute devices. Starting with 1.1.1 plan to start supporting abs devices in some fashion. In the future, we plan to include a configuration file that allows the user to determine which types of devices they want and allow more granual control but without having to remember a moving target like mouse indices or super long usb input names.

Known issue: There is a slow down when combining absolute Apple Magic Trackpads with relative mice. For this reaons absolute devices are ignored. We will revisit this later.

Virtual Multi-Mouse reviews all mouse indices upon startup. This includes its own index, all relative devices, all absolute devices. When a game starts, Batocera inserts its own virtual mouse-keyboard called "evmapy". It will always consume the next available slot. This is usually harmless and usually gets added at the end, but if you remove any usb device, evampy on the next game will take the first available position. VMM is now smart enough to deal with this organized chaos. While we still encourage leaving your usb devices alone while running Batoceara, VMM is king and it can now tame the evmapy lion.

Each version gets better and better! Eventually Virtual Multi-Mouse will literally learn about the games you play and make setup decisions for you. This is slowly being rolled out into each version and so far we've been able to do this with three simple shell scripts. We don't believe this is a bad thing as long as VMM is efficent and works as designed. However, we may start using Rust in the future.

## 🐭👾🖲️ Ready to Enter the Multi-Verse?

0.  If you have smb// working, you can copy files over instead of sneaker net, curl this repo works also
1.  Insert a thumb drive to a Mac or PC 
2.  Format it using ExFat, name the disk `install`
3.  Copy the `MM folder` to the thumb drive
4.  Insert the thumb drive to your Batocera Linux box
5.  Type `F1` to enter File Manager
6.  Navigate to /Applications and open Xterm
7.  `cd /media/install/MM`
8.  `chmod 755 install.sh` #may not be needed
9.  `./install.sh -install`
10.  `reboot`

## 🐭👾🖲️ Manual install instructions coming soon.
0. Until here is a brief summary
1. mm.sh goes in /userdata/system/scripts/ needs `chmod +x` or `755` rights
2. multimouse.sh and custom.sh goes in /userdata/system/ needs `chmod +x` or `755` rights
3. go to terminal, `cd /userdata/system`
4. `./custom.sh` start
5  or `reboot`

## 🐭👾🖲️ Want to Leave the Multi-Verse?

1.  Insert the thumb drive to your Batocera Linux box
2.  Type `F1` to enter File Manager
3.  Navigate to /Applications and open Xterm
4.  `cd /media/install/MM`
5.  `./install.sh -uninstall`
6.  `reboot`

## 🐭👾🖲️ Credits
* Virtual Multi-Mouse developed by StarPlayrX aka Todd Bruss
* KarsMulder for writing Evsieve, simply amazing work
* Special thanks to the Batocera team for giving me a renewed interest in Linux
* Shout out to RetroArch, EmulationStation, Recalbox and MAME teams

## 🐭👾🖲️ Reference Material

* https://github.com/KarsMulder/evsieve
* https://wiki.batocera.org/launch_a_script
* https://forums.libretro.com/t/configuring-ra-for-multi-mouse-spinners-lightguns-tackballs/12619E
* https://forum.batocera.org/d/6652-being-able-to-use-trackball-and-spinner-using-per-mouse-index/27

## 🐭👾🖲️ Coming Soon
* Pacman package manager packages.
