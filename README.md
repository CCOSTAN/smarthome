**Welcome** to my github page. Here you will find a bunch of scripts that I use to automate my home.

I own a bunch of Raspberry Pi's, and Pi Zeros at home. All the software components listing you will see on my github page runs entirely on RPi's. The primary Home Automation software I use is [Home Assistant](https://home-assistant.io/) (HA). It is an open-source home automation platform written by a bunch of smart individuals. Using HA, one can track and control all devices at home. It is a perfect piece of software to run on a Raspberry Pi.

All of the Raspberry Pi's I have at home are wirelessly connected to my home network, and can talk to each other seemlessly via mqtt messaging. Mqtt is used only because it is light weight, loosely couples devices from each other, and provides data persistence. The devices can work independently to each other and can be taken off-line without having to worry - making it easy for me to do plug-and-play work :)

The following picture shows high level architecture of my home network, and what I use for basic automation stuff at home.
![My Home Automation Setup](https://github.com/skalavala/smarthome/blob/master/Home%20Automation%20Setup%20-%20Kalavala.jpg)

Please feel free to let me know if you find any issues with my code, and/or have any suggestions. Thank you!


**Devices I Own currently:**

Wemo Switches
TP Link HS-200 Switches

Wemo Outlets
Eteckcity RF Outlets

Lifx Bulbs
Philips Hue Bulbs

Sharp Aquos Smart TV
Onkyo Receiver

Aeotec ZWave Z-Stick
Aeotec ZWave Multi Sensors

Custom Built Smart outlet - where I used a PiZero and relay switch to turn ON/OFF the electrical outlet. I made a small wooden box to house all the items. It is a poor man's version of smart electrical outlet, but a very smart one, and I have more control over this outlet than the commercial smart outlets.
