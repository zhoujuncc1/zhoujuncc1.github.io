---
layout: post
title:  "Boot Ubuntu Raspberry Pi 4 with legacy monitor"
date:   2021-03-18 09:44:54 +0800
categories: raspberrypi
---
Install Ubuntu for Raspberry Pi 4 with legacy monitor may run into black screen. Solution from internet is 

After burning and SD Card, boot pi with black screen for a while. Take the card back to a computer, modify the `config.txt` under boot parition with following
```
hdmi_force_hotplug=1
config_hdmi_boost=4
hdmi_drive=2
```
Credit to <https://www.raspberrypi.org/forums/viewtopic.php?t=136049#p904864>
