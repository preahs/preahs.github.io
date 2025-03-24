---
title: My Self-Hosting Journey
description: How I started, where I'm at, and where I'm going with self-hosting
date: 2025-03-24 12:07:00 -06:00
categories: [Blogging, Tech]
tags: [writing, informational]     # TAG names should always be lowercase
image:
    path: /assets/img/selfhosted.jpg
    alt: Self-hosting
---

## What is self-hosting?

Self-hosting is the practice of running your own applications or services on hardware you control, like a personal computer, server, or NAS, rather than relying on third-party cloud providers. Essentially, you become your own "cloud" by hosting apps and data yourself. You can avoid subscription fees for services like Google Drive, Spotify, or Netflix by running alternatives yourself. Also, helps you gain hands-on experience with networking, server management, and various technologies.

I was intrigued by self-hosted services for a long time before, but only became interested in hosting my own data and media seriously in 2022 when I naturally gained more technical knowledge over time from schooling and self-research. I had a lot of movies and TV shows I owned on a big external drive, just mp4 or mkv files stored in folders that I could plug into my laptop or PC when I wanted to watch something. 

After getting fed up with streaming service practices, pricing, and unreliablity, I decided to never subscribe to one again and go fully local.

## Plex

Plex is a media server platform that lets you organize, stream, and access your personal collection of movies, TV shows, music, photos, and more across various devices. It works by setting up a Plex Media Server on a computer or NAS (Network Attached Storage), where your media files are stored. Once set up, you can use the Plex app on phones, tablets, smart TVs, game consoles, or through the web browser to access your content just like any other streaming service.

Plex also offers features like automatic metadata fetching (adding cover art, descriptions, and ratings), user profiles, parental controls, and remote access. Additionally, it provides free ad-supported movies, TV shows, and live TV channels. Some premium features, like hardware transcoding and offline downloads, require a Plex Pass subscription. It is probably by far the most popular option for personalized media servers.

### What I like about Plex

- Compatible with most platforms, namely TVs
- Easy to set up and use
- Has its own free media
- Ability to buy Plex Pass as a lifetime fee instead of a recurring subscription

### What I don't like about Plex

- The UI is ugly and cluttered
- Not open-source
- Has some options locked behind paywall
- Not as customizable as I prefer
- Requires creating an account and relies on Plex’s servers, raising privacy concerns.

## Jellyfin

Jellyfin is a free, open-source media server that serves the same purpose as Plex. One of Jellyfin's biggest draws is that it gives you full control over your media without requiring any subscriptions or sending data to third parties. Unlike Plex or Emby, Jellyfin has no premium features locked behind a paywall — everything, including remote access and hardware transcoding, is available for free. Jellyfin also supports features like user profiles, parental controls, live TV, and DVR (with compatible tuners), and it automatically fetches metadata to organize your library. It’s ideal for those who prefer a fully self-hosted solution with complete privacy and open-source flexibility. This is why Jellyfin is my server of choice.

### What I like about Jellyfin

- Default UI is gorgeous, clean, and can be changed to other themes
- Open-source
- Support for various plugins that allow cool features like the ability to [skip intros](https://github.com/intro-skipper/intro-skipper)
- No paywalled features

### What I don't like about Jellyfin

- Fewer official apps, especially on smart TVs and consoles (though you can sideload).
- Remote access and other features require manual setup (e.g., port forwarding)
- Can struggle with very large libraries or heavy transcoding tasks compared to Plex

To be fair, I technically use both. I have both servers on my NAS and point both of them to my media library storage. In this way, I have the option of using either depending on my needs. I usually end up using Jellyfin either way, however.

## My server setup

I tried to go custom with my setup, but my technical knowledge wasn't quite ripe enough. I bought a couple minimal computers off of eBay and installed Linux on them to run my services, but found that they were never powerful enough or otherwise had strange drawbacks. I eventually returned the first and kept the second to be my dedicated Minecraft Machine (works fantastic for running Minecraft servers actually).

My brother and I decided to split the cost to share a [Synology NAS](https://www.synology.com/en-us/support/nas_selector). Synology is a Taiwanese company that specializes in NAS devices, as well as software solutions for data management, surveillance, and networking. They’re widely recognized as a leader in the NAS market due to their combination of user-friendly software, robust hardware, and a feature-rich ecosystem.

Synology’s web-based operating system, DiskStation Manager (DSM), is incredibly intuitive, making setup and day-to-day management accessible even for non-techies. DSM feels more like a desktop environment than a traditional NAS interface, providing tools to manage storage, apps, and devices much easier than other custom options. Additionally, QuickConnect simplifies remote access without needing port forwarding.

So far it has been perfect for my needs. My brother bought his own SATA drive, I bought my own, and slotted them in. He backs up his information on his and I use my drive for all of my data. I installed the Synology Drive client on my desktop and laptop, which acts just like Google Drive or Dropbox, so I can access D&D sheets or schoolwork from anywhere across multiple devices.

I set up Jellyfin and Plex using [Docker](https://www.docker.com/), which comes pre-installed in the container manager (can I just say how amazing Docker is for self-hosting? If I don't like a service, I can wipe it out in one go). I recently set up [Audiobookshelf](https://www.audiobookshelf.org/) as well, which has been a truly _amazing_ audiobook solution. I can listen to any of my owned audiobooks (of which I have many) from my phone any time without any interruptions and with chapter navigation, just like Audible. It also has podcast support, but I haven't had reason to try that out yet.

I have more I desperately want to try, but between school and work I don't have as much time to tinker with it. Here are my WIP or future ideas:

1. [Immich](https://immich.app/). Open-source photo and video backup solution.
2. [Calibre-web](https://github.com/janeczku/calibre-web). Similar to Audiobookshelf but with ebooks.
3. [Pihole](https://pi-hole.net/). Network-wide adblocker. I have this setup on my Raspberry Pi, but having it on my NAS instead might be preferable, especially if I set it up so that my phone can access the adblocking capability anywhere.
4. [Mealie.io](https://mealie.io/). Open-source recipe manager and meal-planning app designed to help you organize recipes, plan meals, and generate shopping lists.
5. [Actual](https://actualbudget.org/). Open-source personal finance and budgeting tool.


Who knows how much more I'll get into. I also want to delve into making my services externally available without using [Tailscale](https://tailscale.com/), to more easily share this with friends, but that's a whole thing. Exposing data to the internet without taking the proper precautions could result in my server being hacked or scraped for data.

Don't get me wrong, Tailscale is one of the best options out there for a private network. I use it all the time, for Minecraft servers, for my current NAS setup. But exploring other options would be a very exciting area to learn about.

This post may be updated as I progress in my self-hosting goals.
