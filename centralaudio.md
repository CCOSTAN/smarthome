##Poor man's version of Multi-room Audio System

I have always wanted to have a centralized audio system for my home, since my home is not currently wired for that, I have two choices  - get a commercial central audio system by spending a boat load of money, or make my own. I chose to build my own with a bunch of Raspberry Pi devices, some {cheap} bluetooth speakers from amazon and leverage old speakers lying at home.

The way it works now is pretty simple. My primary Home Automation Server (Raspberry Pi), running Home Assistant software also runs Mopidy, Snapcast Server components. In each room, I have a Raspberry Pi physically connected to a speaker, that runs snapcast client software. All the Raspberry Pi's are connected to the same network/subnet. This set up allows me to play music across all the rooms, as well as it allows me to annouce any Home Assistant related messages/events. Since I have mopidy (mpd) configured in my Home Assistant, I can pause, play media and automate anyway I like it.

Here is the picture - of my "Smart" Multi-Room Audio System:

![My Smart Whole House Audio System ](https://github.com/skalavala/smarthome/blob/master/images/MultiroomAudioSystem-Kalavala.jpg)
