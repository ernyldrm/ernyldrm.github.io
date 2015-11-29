---
layout: post
title: How to create your home media server using Raspberry Pi 2
redirect-from: 2015/10/08/home-media-server
permalink: raspberry-pi-media-server
---

Hello everyone,

In this post I'm going to tell you about how I managed to create my own home media server using new Raspberry Pi 2. 
It's got 1 GB of RAM and a new Broadcom CPU, so a lot of potential to install a greater workload to the pi. So stay with me.

![Raspberry Pi 2](/public/raspberry-pi-2-angle-100569133-orig.png)

### My Setup:

- A Raspberry Pi 2
- A 3TB Toshiba Canvio External HDD with NTFS (Powered separately)
    - Powering your HDD from your Pi can cause problems. HDDs need a bit more power than what pi can provide
- An 8GB Micro SD card from SanDisk (Class 10 + UHS-1 Support)
- A 2.1 amps USB adapter for powering the pi

### Setting Up the Operating System

Raspbian is the Foundation’s official supported operating system. And that's the OS of my choice, because everything is just tailored for the pi. 
I preferred the "wheezy" distro earlier, because the linux kernel version seemed to be more stable and compatible with the software I will use. 
But then I realised "jessie" can run all of them. So grab the distribution of your choice from [here](https://www.raspberrypi.org/downloads/raspbian/)
(you can also download the jessie lite if you dont require most of the software pi provides) and head to this [tutorial](http://blog.self.li/post/63281257339/raspberry-pi-part-1-basic-setup-without-cables) to install raspbian without 
a keyboard, mouse or a monitor. In my case I didn't have any of those on hand. 

    If you are using a Windows Environment to control Raspberry Pi, you can use PuTTy terminal to ssh into your device. 
    Otherwise if you are on a mac or linux environment you can just open up your terminal and directly ssh into your terminal.

### Mount your HDD automatically on startup

After deploying your OS and do all the initial configuration, you are ready to mount your hdd. If you don't have an external HDD, skip this part.
But for intensive torrent downloading you will need an HDD. Simply, follow [this tutorial from HTPC Guides](http://www.htpcguides.com/properly-mount-usb-storage-raspberry-pi/)
to learn how to. You may use your usb powered hdd but it may cause some issues and device may randomly disconnect due to power insufficiency (or may never connect properly)

    If your drive is using ntfs, I personally use ntfs-3g to mount it, despite what tutorials says.

### There is more to come

I've setup most of the things needed right now but I'm trying test everything out better to serve the best tutorial here. More to come in a few days.