---
layout: post
title: Windows 10 IOT Core and Raspberry PI
---

Setting up the Raspberry Pi with a default install of the Windows 10 IOT Core OS appears to be a pretty straightforward process. There are some slick looking introductory pages in the Windows Dev Center
to get you started, however, I ran in to a few gotcha's along the way. 

I've pulled together the resources I used, and documented the steps that caught me out, to hopefully make the experience a little easier in future. 

**Goal**

* To install the Windows 10 IOT Core operating system to a Raspberry Pi 3, and deploy a 'Hello World' Universal Windows Platform app to the device. 


**Prerequisites**

* Main PC Operating System - Windows 10
* Install <a href="https://www.sdcard.org/downloads/formatter_4/eula_windows/" target="_blank">SD Formatter 4.0</a>
* Unlock the Administrator Account on your Windows 10 machine

**Steps**

1. Log in as the Administrator user on your machine
By default the Administrator account is disabled out of the box when you install Windows 10, following these steps to activate the account
2. Go to MSDN
3. Download the Windows IOT Dashboard
* Run the IOT Dashboard, logged in as the Administrator account (not just as elevated administrator priviliges)
* Run SD Formatter 4, run full format with the option turned on
* Otherwise you will have failures unpacking the image to your SD card

*In Visual Studio*

* Install the UWP extensions
* Setup your hello world app
* Debug to a remote device
* All good?
* Change to release, rebuild the solution and hit deploy

*Powershell*

Setup a powershell session to remotely connect to your PI

* Set your new app to be the startup app
* Reset your device
* Walah

* To revert back to the default app, run IOTCoreDefualt


![_config.yml]({{ site.baseurl }}/images/productivity.jpg){: .post-img }





