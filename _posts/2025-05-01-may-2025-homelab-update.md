---
title: May 2025 Homelab Update
description: Update on my homelab for May 2025!
date: 2025-05-01 21:45:00 -06:00
categories: [Homelab, Update]
tags: [homelab, technical]     # TAG names should always be lowercase
image:
    path: /assets/img/server_back.jpeg
    alt: My Dell PowerEdge R730
---
I have made quite a bit of progress on my homelab since my post about general self-hosting plans. I still have my Synology NAS, and will be keeping it as a backup solution. You can never have too many backups.

I recently purchased a used Dell PowerEdge R730, which is a 2U rack-mounted enterprise server designed for data center and business-critical workloads. For me, it's a great noise-making machine that has lots of upgrade potential! Here is the boring technical details:

- 8 Bay 2.5" SFF
- H730 Raid Adapter
- Dual Xeon Processors
- Dual 750W PSU
- Total PCI Express X8 Slots: 3
- Optical Drive Type: DVD Player
- Number of Processor Cores: 16
- Total PCI Express X16 Slots: 1
- Memory Type: DDR4
- Memory Frequencies Supported: 1333, 1600, 1866, 2133
- Total USB Ports: 4
- Processor Series: Intel Xeon E5
- Total Serial Ports: 1
- Server CPU Model: E5-2667 v4
- Maximum # of Hard Drives: 8
- Total Memory Slots Available: 24
- Server Series: PowerEdge R730
- LAN Compatibility: 10/100/1000 Gigabit
- Maximum Hard Drive Size Supported (GB): 43200
- CPU Socket: Dual LGA 2011
- Front USB 2.0 Ports: 2
- Total Hot-Swap Bays: 8
- Total RAM (GB): 16
- Maximum Memory Supported (GB): 768

![Desktop View](/assets/img/server_front.jpeg){: width="240" height="108" }
_Front of the server_

![Desktop View](/assets/img/server_back.jpeg){: width="240" height="108" }
_Back of the server_

Yes, I have it on a table on wood blocks instead of a rack for now. I swear I'll buy a rack soon when I have the funds. I just also have 8 drives and a surge protector that can handle the power draw on my wishlist 🫠.

Upon arrival, I had to buy two power cables and a BOSS adapter with an M.2 SSD. Then I was good to install an operating system. I frequent the reddit communities [r/homelab](https://www.reddit.com/r/homelab/) and [r/selfhosted](https://www.reddit.com/r/selfhosted/), and decided to use Proxmox VE based on recommendations. I installed Proxmox VE 8.4 onto a USB stick and plugged it into the server, then installed the OS from the iDRAC interface from my desktop computer.

I was really pleased to find out that iDRAC exists. iDRAC, which stands for Integrated Dell Remote Access Controller, is a proprietary technology developed by Dell that provides out-of-band management for Dell servers. It allows system administrators to remotely monitor, manage, update, and troubleshoot servers regardless of the operating system status or even whether the system is powered on or not! iDRAC functions independently of the server’s primary CPU and operating system by using a dedicated network port, which means administrators can access the server even if it is unresponsive or offline. That means it was much easier than initially expected to log onto it and power it off and on remotely. I can even see a virtual depiction of the screen on my desktop and make selections from there.

![Desktop View](/assets/img/server_idrac.jpeg){: width="240" height="108" }
_The iDRAC port_

Proxmox was pretty overwhelming at first. There are so many options, since it's such a powerful operating system and hypervisor. I messed around with some LXC containers before I found out there is this extremely useful tool called [Proxmox VE Helper-Scripts](https://community-scripts.github.io/ProxmoxVE/scripts). It's a community led database of scripts that automate the process of installing self-hosted services such as Jellyfin, Plex, Karakeep, Pi-hole, Cloudflared, Tailscale, and more. I have been making a lot of use out of this, and used those to so far install Cloudflared, Karakeep, Paperless-ngx, Pi-hole, and Tandoor.

I used to use Mealie for recipe management, but I decided to give Tandoor a go. I wouldn't say I super prefer one over the other, honestly. I suppose I prefer mealie's uncomplicated UI and how it breaks down prep steps, but Tandoor labels recipes with prep times from the front page and lets you adjust serving sizes which I really like. It's what I'm going with for now. I added it as a subdomain to my Cloudflare tunnel, meaning I can access it remotely from anywhere easily and log in to view my recipes. My friends and family can do the same too, if I send them an invite link to create a user.

I set up Pi-hole and now have adblocking network-wide again. It usually didn't affect me before, but it feels nice knowing that my family's devices won't be sending all that telemetry data anymore. 

There's more to come and more to learn. I have been documenting everything so far on Obsidian for easy reference. Once I am able to buy more hard drives, I can set up the most important part: streaming and other media libraries.