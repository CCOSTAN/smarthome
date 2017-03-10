**Poor man's version of Central Audio System**

I have always wanted to have a centralized audio system for my home, since my home is not currently wired for that, I have two choices  - get a commercial central audio system by spending a boat load of money, or make my own. I chose to build my own with a bunch of Raspberry Pi devices and some cheap bluetooth speakers from amazon.

The way it works now is my primary Home Automation Server(Raspberry Pi), running Home Assistant publishes frequent updates, statuses, announcements...etc to a specific topic on the local MQTT server. I then have Raspberry Pi's in each floor that are on the same network, subscribes to that topic and receives the messages instantly. 

Based on the tracker information and motion sensor data, the individual RPi determines what to do with that data. For e.g. when people are not home, there is no reason to play the audio or call test-to-speech and play the announcements. Similarly, when people are home, and no motion detected upstairs, and TV is on downstairs, it will only play the audio downstairs and not upstairs.

Currently this setup is only used for announcements around the house. My next step would be to use the same setup to play music across the rooms using `snapcast` and `Gstreamer`.

Here is the set up of my poor man's smart central audio system design:

![My Centralized Audio Setup ](https://github.com/skalavala/smarthome/blob/master/Central%20Audio%20System%20For%20Home%20-%20Kalavala.jpg)
