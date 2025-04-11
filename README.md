# Introduction 
This is a collection of scripts I use (for the most part, in conjonction with dmenu).

## 0x0
A simple wrapper to https://0x0.st/. Uploads the file provided in argument with a expiry timer of 1 hour and prints the URL. 
## battery-check
A very simple script that checks the battery level and creates a notification via ```notify-send``` when the battery level is under 20% or at 89%.
## volumecontrol
General volume control script for PulseAudio using ```pactl```. Increments/decrements audio by 5%, and mutes/unmute depending of the flag provided. Creates notifications on change with ```notify-send```.
```bash
volumencontrol [-idth]
  -i: Increments volume by 5
  -d: Decrements volume by 5
  -t: Toggles volume between mute and unmute
  -h: prints this help section
```
## snapshot
General screenshot/video capture script using ```scrot```, ```dmenu```, ```x11grab``` and ```ffmpeg```. Prompts the user to select a region using ```scrot``` (and a duration via ```dmenu``` for video capture), and saves a screenshot in .png format, or a recording in .mp4, in a user-defined directory.
```bash
snapshot [-svh]
  -s: screenshot mode
  -v: video capture mode
  -h: prints this help section
```
## storagesync
A simple storage sync script using ```rsync``` with different presets depending on the device mounted.
```bash
storagesync [-abgh]
 -a: audio mode
 -b: books mode
 -g: general mode
 -h: prints this help section
```
## vpn
Simple utility to toggle a WireGuard interface through nmcli.
```bash
vpn [-ht]
-t: toggles the vpn
-h: print this help section
```
