The goal of this project is to build a presence detector for five friends living together. Using the wifi capabilities of a ESP8266,
this microcontroller is looking for this five known MACs of the wifi adapter of their smartphones. If a MAC is near the ESP8266, 
a green LED (of friend #1) is switched on, otherwise another LED is red and so on, til I get this result:


Example:

+--------------------------------+
|                                |
|   #1    #2    #3    #4    #5   |
|                                |
|   RED   RED   RED         RED  |
|                                |           Result: #4 is available for drinking beer!
|                                |
|                     Green      |
|                                |
+--------------------------------+




# Friend Detector by Ricardo Oliveira, forked by Skickar 9/30/2018

This project requires: A NodeMCU, a mini-breadboard (or full sized one), and a 4 pin RGB LED. 

 The function of this code is to read nearby Wi-Fi traffic in the form of packets. These packets are compared to a list of 
 
 MAC addresses we wish to track, and if the MAC address of a packet matches one on the list, we turn on a colored LED that is 
 
 linked to the user owning the device. 

 For example, when my roommate comes home, the	transmissions from his phone will be detected and cause the blue LED to turn on 
 
 until his phone is no longer detected. It can detect more than one phone at a time, meaning if my phone (red) and my roommate's phone (blue) are both home, the LED will show purple. 

## For more information on the design go to: https://www.hackster.io/ricardooliveira/esp8266-friend-detector-12542e

