---
title: I ordered an SSD enclosure from AliExpress
slug: ssd-enclosure-issues
description: ...and it didn't connect to Windows at all. Bummer.
tags:
date: 2025-09-29T14:54:41+05:00
draft: true
image:
layout:
excludeSearch: false
unlisted: false
---
I love AliExpress.

I have ordered so many niche things (circuit boards, modules, accessories), that aren't that readily available in my country. Even a Torx screwdriver once! (I was too lazy to go and find it from a hardware shop.)

After the recent price hike and the surge in prices, I decided to take a risk and order an SSD enclosure. I have the base model Mac mini and it only has 256GB storage which runs out faster than you can say "256GB is probably enough for me." 

Since video projects take up a lot of space, and an external storage with ridiculous read/write speeds is the way to go. Particularly an NVMe enclosure. Now, the locally available options were at max 5Gbps. Too slow. And AliExpress takes a decade to deliver. Moreover, the Samsung T7 or T9 does not give amazing speeds on Mac (blame the whole USB vs Thunderbolt standards mess). 

After much scouting, I realized I needed an enclosure that has good heat dissipation because of high ambient temperatures where I live, and the fact that SSDs get incredibly hot and throttle their speeds. Many tabs later, I settled on the Meetiger 40Gbps NVMe Enclosure. It had good reviews on the product page, with people quoting speeds greater than 3000MB/s. And it was on sale. Naturally it seemed like the best option. The only caveat was that it had no online reviews, on YouTube or Reddit. Red flag. But the reviews on the page were enough of a social proof to give me the ease of mind. 

Fast forward a month later (after being stuck in customs for over a week), I received my package. 

_picture of package_

The unboxing experience was nice, they included some thermal pads and a screwdriver to help with the installation of the drive. As well as a Thunderbolt cable, and a USB3 A-to-C cable. Everything was included. Props to them. No email address or website on the box tho. Second red flag. 

I was super excited to open it up and test it. I inserted a Samsung SSD from an old laptop into it and plugged it into my Mac. It was read only tho — NTFS. No worries. Formatted to exFAT, ran a test and viola! 

_picture of blackmagic test_

Consistent 3000MB/s+ Read speeds with 1500MB/s+ write speeds (the SSD's max limit). I was pleased with my purchase. Everything seemed to work with no issues whatsoever (I was expecting SSD compatibility issues because many forums claimed some SSDs don't play well with the enclosure's hardware). 

Vindication. Everything is working as it should, right? 

Well...no.

I plugged in the enclosure into my Windows laptop. I see a light on the enclosure. And it goes out. I see an exclamation mark in Device Manager. Okay maybe a driver issue. Maybe the wrong port. 

After many trials and tribulations (changing ports and researching online), I found out that Windows is a bit more picky when it comes to external NVMe storage which uses the USB Attached SCSI (UAS), or UASP protocol.