**Welcome** to my github page. Here you will find a bunch of scripts that I use to automate my home.

I own a bunch of Raspberry Pi's, and Pi Zeros at home along with a bunch of "smart" devices. All these smart devices work great independently, and my goal is to bring all of them together and have them talk to each other with a little bit of programming and make them really smarter! I also want to be able to run all the software on Raspberry Pi only. I have no interest in investing in additional computing hardware. 

The primary Home Automation software/platform that I use is [Home Assistant](https://home-assistant.io/) (HA). It is an open-source home automation platform written by a bunch of smart individuals. HA allows you to track and control devices easily with simple configuration and with a little bit of scripting, you can do wonders. It is also a perfect piece of software to run entirely on a single Raspberry Pi.

All the Raspberry Pi's I have at home are wirelessly connected to my home network, and can talk to each other seemlessly via mqtt messaging. Mqtt is heavily used at home because it is light weight, loosely couples devices from each other, provides data persistence and security. The devices can work independently to each other and can be taken off-line without having to worry - making it easy for me to do plug-and-play work and make changes on the fly :)

The following picture shows high level architecture of my home network, and what I use for basic automation stuff.
![My Home Automation Setup](https://github.com/skalavala/smarthome/blob/master/images/Home%20Automation%20Setup%20-%20Kalavala.jpg)

Please feel free to let me know if you find any issues with my code, and/or have any suggestions. Thank you!


**Devices I have currently:**

* Wemo Switches

* TP Link HS-200 Switches

* Wemo Outlets

* Eteckcity RF Outlets

* Lifx Bulbs

* Philips Hue Bulbs

* Sharp Aquos Smart TV

* Onkyo Receiver

* Home Security System

* Aeotec ZWave Z-Stick

* Aeotec ZWave Multi Sensors

* Bunch of Raspberry Pi's

* Bunch of Pi Zero's

* Cheap Bluetooth speakers from Amazon

* Radio Frequency Transmitters and Receivers

* Sensor kit from Raspberry Pi for experimentation - 

Custom Built Smart outlet - where I used a PiZero and relay switch to turn ON/OFF the electrical outlet. I made a small wooden box to house all the items. It is a poor man's version of smart electrical outlet, but a very smart one, and I have more control over this outlet than the commercial smart outlets.
