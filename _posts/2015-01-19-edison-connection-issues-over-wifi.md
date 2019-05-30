---
title: Edison connection issues over wifi
published: true
categories:
  - Blog
tags: 
 - Intel
 - Edison
---

I've been trying to get up to speed with the excellent [cylon.js](http://cylonjs.com/) library for a while now so finally carved out some time to try to set it up and running on an [edison](http://www.intel.co.uk/content/www/uk/en/do-it-yourself/edison.html) board and the [Intel XDK](https://software.intel.com/en-us/html5/xdk-iot) IDE but I ran into a very fundamental roadblock...I couldn't connect my laptop to the Edison over my home wifi network (which by normal [means](https://github.com/mashery/edison-guides/wiki/Intel-Edison-Wi-Fi-Guide) is a pretty easy process).

I tried various solutions from the Intel support [community](https://communities.intel.com/) but after trying it with different laptops and networks where it worked with no issues, it became clear that the issue lay somewhere in my home network.

After trying various different configurations, I found the root turned out to be the fact my wireless router was using automatic channel selection. The solution was found when I tried to set up Airdroid to try to find if my mobile could also connect to my laptop over wifi. When I switched this to use a specific channel, all my problems disappeared. __Awesome!__

Hopefully I'll have some follow on articles in the near future but, yes, I did get an LED blinking :D