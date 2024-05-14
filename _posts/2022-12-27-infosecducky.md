---
layout: post
title: Would Your Users Plug In A Random USB?
author: chris
date: 2022-12-27 14:30:00 -0500
categories: [Portfolio, Coding Projects]
tags: [portfolio, coding projects, cybersecurity, duckyscript, flipperzero]     # TAG names should always be lowercase
image: assets/images/53.png
  
  


---
# Cyber Security Tools - Mac Ducky Script Red Team Security Test

 
I made this Ducky Script for testing if end users will plug in a random usb (ducky) or cable(O.MG).

1) When the device is plugged in, the payload triggers. It collects the logged in user name and the serial number of device.

2) It then sends that info to a discord webhook

<div style="display: flex; justify-content: center;">
  <img width="333" src="https://user-images.githubusercontent.com/112792126/209692167-1a0081d4-9446-42cb-bf51-5d1c93d0711c.png">
</div>
<br/><br/>

3) User gets a popup telling them they failed the evaluation and to return the device to the team.

<div style="display: flex; justify-content: center;">
  <img width="333" src="https://user-images.githubusercontent.com/112792126/209692487-6c9de450-f84f-409e-8b7a-c84e0d31144e.png">
</div>

  <br/><br/>
# Technology Used

- Understanding of MacOS & Bash/Shell
- Duckyscript to write code
- Discord Webhooks
- O.MG Cable & Flipper Zero (BadUSB) to test script deployment
