---
title: 'Raspberry pi and the power problem '
published: true
categories:
  - Blog
tags: 
 - Raspberry Pi
---

The Raspberry Pi really is an amazing device and it's not hard to see why this excellent device is the tool of choice for getting kids and other enthusiasts up and running with computers. Hey, many of the OS's come with some version of Mine Craft installed!

I recently was trying to set up the Raspberry Pi 2 model B and I unfortunately was having issues during the installation. I'd tried a couple of different approaches including initially trying the Noobs installer, then the Raspbian image itself and was each method was failing at a different point, but both were failing pretty early in the installation process.

I was trawling through the forums and the two different possible sources, the SD card or the power supply. It turns out the Raspberry Pi 2 is pretty inconsistent in it's behavior of the power supply is not good. I switched to another USB power supply and the install finished smoothly. 

So it got me thinking of whether or not your average, non multi-meter carrying human could see what their power supply was like and thankfully the [Google Play Store](https://play.google.com/) came to the rescue. I installed an app for measuring the effectiveness of your charger (both the Pi and Android phones using micro-usb cables) and plugged in the original power supply to my android phone and got a reading of roughly 250mA. When I switched to the second power supply I got a reading of over 1250mA.

A couple of good resources to look at before you despair too much:

[http://elinux.org/RPi_SD_cards](http://elinux.org/RPi_SD_cards) - list of many SD cards and record of whether there are any known issues with it and it's use with Raspberry Pi.
[https://play.google.com/store/apps/details?id=com.gombosdev.ampere](https://play.google.com/store/apps/details?id=com.gombosdev.ampere) - Android application for measuring how much charge your power and cable are actually delivering.