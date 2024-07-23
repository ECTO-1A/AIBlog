---
featured: true
layout: post
title: Crashing iPhones with Flipper Zero and The Story Behind CVE-2023-42941
author: chris
date: 2024-01-20 14:30:00 -0500
categories: [Cybersecurity, Coding Projects]
tags: [portfolio, coding projects, mac, ios, ble]     # TAG names should always be lowercase
image: assets/images/66.png
---

### Crashing iPhones with Flipper Zero: The Story Behind CVE-2023-42941

It's been a whirlwind since I uncovered a significant vulnerability in Apple's Bluetooth protocol, earning CVE-2023-42941. My work on reverse engineering Apple's BLE has sparked widespread attention, especially with the notorious Flipper Zero device at the center of it all.

#### The Infamous Flipper Zero iPhone Crash

The Flipper Zero, originally designed as a multifunctional tool for penetration testing and hobbyist projects, gained notoriety for its ability to exploit a BLE vulnerability in iPhones. By spoofing BLE advertising packets, the Flipper Zero could spam iPhones with continuous pairing requests, causing them to freeze and reboot.

This exploit turned the Flipper Zero into a Denial-of-Service (DoS) weapon against iOS devices. The vulnerability affected various Apple services that rely on BLE, such as AirDrop, Handoff, and connecting to Apple TV. Despite several iOS updates, including iOS 17.2, Apple struggled to mitigate this exploit effectively.

#### Real-World Impact

The impact of this exploit wasn't limited to technical demonstrations. There were numerous reports of disruptions in schools and public places. Students were suspended for using the Flipper Zero to crash iPhones, causing significant chaos and drawing attention from major tech sites ([9to5Mac](https://9to5mac.com/2023/12/15/the-jig-is-up-flipper-zero-devices-can-no-longer-crash-iphones-running-ios-17-2/), [Malwarebytes](https://www.malwarebytes.com/lock-and-code-podcast/flipper-zero-iphone-crash), [MacRumors](https://www.macrumors.com/2023/12/02/apple-fixes-flipper-zero-iphone-crash/), [Gizmodo](https://www.gizmodo.com.au/2023/12/apple-shuts-down-flipper-zeros-ability-to-shut-down-iphones/)).

One notable incident involved Jeroen van der Ham, who experienced the exploit firsthand on a train in the Netherlands. His iPhone, along with those of other passengers, was bombarded with pairing requests, rendering the devices unusable until they were rebooted. This highlighted the severity and potential misuse of the vulnerability.

#### Setting the Record Straight

While some credit went to the moniker "Techryptic" in several articles, I want to clarify that this research and the resulting exploit stem from my work under the username "ECTO-1A." The discovery of the BLE flaw and its potential for disruption was a culmination of my extensive research into Apple's BLE protocols.

#### Apple’s Response: iOS 17.2 Update

In response to this widespread issue, Apple released the iOS 17.2 update in December 2023, which implemented safeguards to prevent Flipper Zero devices from crashing iPhones. According to tests by [9to5Mac](https://9to5mac.com/2023/12/15/the-jig-is-up-flipper-zero-devices-can-no-longer-crash-iphones-running-ios-17-2/) and [ZDNet](https://www.zdnet.com/article/ios-17-2-update-puts-an-end-to-flipper-zero-iphone-shenanigans/), iOS 17.2 has successfully mitigated the exploit. While the devices might still receive a few pop-ups, they no longer crash or reboot as they did before.

The update appears to introduce a timeout mechanism for BLE advertising packets, effectively stopping the flood of pairing requests that led to the DoS attacks. This fix has significantly reduced the exploit's impact, transforming it from a severe vulnerability into a minor annoyance.

#### Moving Forward

The Flipper Zero iPhone crash exploit serves as a stark reminder of the importance of robust security measures in our increasingly interconnected world. For now, the best protection against such attacks is to disable Bluetooth if you notice unusual pop-ups, although this is far from a perfect solution.

As for Apple, the company needs to address these vulnerabilities comprehensively. While the Flipper Zero's capabilities are impressive for educational purposes, they also underscore the critical need for security in consumer devices.

Feel free to explore my [**AppleJuice**](https://github.com/ECTO-1A/AppleJuice) repository on GitHub for more insights into BLE security and my ongoing projects. Let’s continue to push the boundaries of what we can learn and achieve in the realm of Bluetooth security. And remember, with great power (or a Flipper Zero) comes great responsibility. Happy hacking!