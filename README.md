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
  -i: Increments volume by 5.
  -d: Decrements volume by 5.
  -t: Toggles volume between mute and unmute.
  -h: prints this help section
```
