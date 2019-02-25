

# 1.21 Arcade Edition
-------

## Rationale
1.21 Arcade Edition uses OpenNode. Set up a free account here 
https://opennode.co/join/f774f2a0-1377-45e2-b719-6b821f24900d

## Purpose
Ever since I got into Bitcoin I wanted my pinball machine to accept Bitcoin payments. Just accepting Bitcoin from friends or to show as an example how to pay. But accepting bitcoin for a pinball game isn't working for the arcade. They need something cheap fast and simple to implement. With lightning and Opennode now you can set this up pretty simple and cheap. 

The purpose of this guide is step by step tutorial so everyone can make this module and implement it in an arcade machine. If it accepts coins it can also accept Lightning.

## Hardware needed

* ESP32 (without built in OLED!)
* MH-ET-LIVE epaper module 
* Relay
* Wires and stuff

## Optional Hardware
Because I'm putting my module in a Williams Jackbot pinball machine I will also be using the following:
* small breadboard
* 12v to 5v buck converter
* molex 15 pin 0.156" female connector
* more wire with dupont connectors

## Setting up
...add instructions how to setup the ESP32, Epaper and relay for testing...

## Installing Arduino IDE
Now sorry for everyone who knows how to upload code to boards. 80% of this step is not needed for you.

To program the ESP32 we need to install Arduino IDE. Once installed you need to add the ESP32 boards into the boardmanager.
Go to File/Preferences and add this link to Additional Boards Manager URLs: 
https://dl.espressif.com/dl/package_esp32_index.json
Click ok and now go to Tools/Boards/Boards Manager. Search for and install ESP32 by Espressif Systems.

Now we need to install some libraries. Go to Tools/Manage Libraries (Ctrl+Shift+I) and install:
* ArduinoJson by Benoit Blachon v5.13.4 (don't install the beta version!!)
* GxEPD2 by Jean-Marc Zingg
* Adafruit GFX Library by Adafruit
* QRCode by Richard Moore

## The code
With all the libraries needed installed we can go to the code for the ESP32.



## Limitations 

I'm an imbecile. This project would not have been possible without the kind help from folks at Fulmo's lightning-network hackdays http://fulmo.org/. The project has been developed for demonstration purposes only, although it is surprisingly stable, and with a little work the project could be secure and production ready. 


