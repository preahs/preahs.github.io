---
title: Switching To Linux
description: A general guide to switching your operating system to Linux, and why.
date: 2025-08-10 14:40:00 -06:00
categories: [Guides, Tech]
tags: [informational, large]     # TAG names should always be lowercase
image:
    path: /assets/img/switchtolinux.png
---
Depending on the type of people you hang out with, you may have received this recommendation before. But how feasible is this, really? And how technical do you need to be to do this? The short answer is, depending on how you use your computer, it can be very feasible and not that difficult, and has only become easier.

## What is Linux?

Linux is a free and open-source operating system based on Unix, originally created by Linus Torvalds in 1991. It is known for its stability, security, and flexibility, making it popular for everything from servers and supercomputers to smartphones and personal desktops. At its core, Linux is a kernel, which is the central part of the operating system that manages hardware and system processes, but it’s typically used in combination with other software to form a complete operating system, often referred to as a Linux distribution (or "[distro](https://en.wikipedia.org/wiki/Linux_distribution)").

Examples of popular distributions include Ubuntu, Fedora, Debian, and Arch Linux. Because its source code is open, Linux allows anyone to inspect, modify, and contribute to its development, fostering a large, active global community of developers and users. This openness and versatility make Linux a powerful choice for both everyday users and advanced technical wizards.

## How does it compare to other, more popular operating systems?

It can vary hugely or not so much depending on which distro you go with. Some types are meant to run only as servers, accessed only from the command line interface (CLI), while others are meant to be an all-in-one package with everything you need to start using your computer without much tinkering. The fun part is there are so many options, and if you like tinkering, you can customize it to do **whatever you want**. This will be mainly geared toward people who like to turn on their computer and just use it, but my enthusiasm will no doubt leak through.

While Windows and macOS are proprietary and developed by single companies (Microsoft and Apple, respectively), Linux is developed collaboratively by a global community, giving users far more control over the system. This makes Linux ideal for developers, system administrators, and privacy-conscious users. However, it tends to have a steeper learning curve, especially for those used to graphical user interfaces and plug-and-play software found in Windows or macOS.

Linux also supports a wide range of hardware and can be run efficiently even on older or low-powered devices, whereas other OSes often require more system resources. In terms of software compatibility, Linux does not natively run many popular commercial applications or games designed for Windows or macOS, though alternatives or workarounds (like Wine or virtual machines) often exist.

## Windows is known as being the best for gaming, what about Linux?

I still agree that if you are a major gamer, *especially* for multiplayer games with anti-cheat, Windows is the better option.

> See [Are We Anti-Cheat Yet?](https://areweanticheatyet.com/) to get an idea of what games you can and cannot play on Linux due to anti-cheat restrictions.
{: .prompt-tip }

However, gaming for Linux has been revolutionized by [Valve](https://www.valvesoftware.com/en/), the creators of [Steam](https://steampowered.com/). The most significant step came with the development of Steam for Linux, which launched in 2013 and brought a curated selection of native Linux games to the Steam platform. However, Valve’s real revolution began with the creation of Proton, a compatibility layer based on Wine that allows Windows games to run on Linux with little to no modification. Integrated directly into the Steam client, Proton enables thousands of Windows-only titles, including major AAA games, to run on Linux with good performance and stability.

Valve has also contributed to the broader open-source ecosystem to improve gaming on Linux, investing in graphics drivers (especially for AMD GPUs), collaborating with developers to enhance Vulkan (a high-performance graphics API), and supporting tools like DXVK (which translates DirectX to Vulkan). These efforts have significantly closed the performance gap between Linux and Windows for gaming.

The launch of the Steam Deck in 2022, a handheld gaming device running SteamOS (a Linux-based operating system), marked another major milestone. The Steam Deck proved that Linux could be a foundation for a mainstream gaming device, delivering a seamless gaming experience without relying on Windows. Altogether, Valve's contributions have not only made Linux more gamer-friendly but have also encouraged game developers and publishers to consider Linux compatibility as a legitimate part of their release strategy. In my opinion, things will only improve from here for Linux gaming.

> Check out the long-running website [GamingOnLinux](https://www.gamingonlinux.com/) for the latest news about gaming on Linux.
{: .prompt-tip }

I'll give my personal experience. My main operating system is Linux Mint, one of the most user-friendly distros, and I can play every game I want on it. Heck, because I'm deranged, I modded Skyrim with 1500+ mods and it can run with minimal issues. By adding a repository for the most up to date NVIDIA drivers, I am able to use the most up-to-date and bleeding edge graphical drivers for my GPU. Additionally, using Proton, I can play pretty much any game in my library using Proton for compatbility, and add an executable or other Windows-only program to Steam to let it use the same compatibility layer. This works for me because I don't play multiplayer games and am willing to tweak things.

I also own a Steam Deck, and am able to play Baldurs Gate 3, Oblivion Remastered, Cyberpunk, Skyrim, Stardew Valley, and more on it. I love my Steam Deck and highly recommend it.

After considering your gaming habits, you can decide on what you want to go with. If you have decent storage, you can actually dual-boot linux *alongside* Windows, giving you access to both operating systems.

## Programs to use on Linux. Go free and open-source!

The main point of Linux is its freedom and that it is free and open-source. Consider some alternatives to your most frequently used programs if deciding whether to make the switch.

1. **Microsoft Office ➜ LibreOffice**
   - LibreOffice is a powerful, full-featured suite with word processing, spreadsheets, and presentation tools. It is very similar to MS Office and completely free.
2. **Microsoft Edge ➜ Firefox or Chromium-based**
   - Firefox is privacy-focused and open-source. Compare and contrast browsers in this same post, further up.
3. **Adobe Photoshop ➜ GIMP (GNU Image Manipulation Program)**
   - GIMP is a powerful raster graphics editor. It has a learning curve but offers many advanced features. I'm not going to pretend that it's *as good* as Photoshop, especially if you use Photoshop every day or professionally, but once you get past the learning curve it can be very comparable.
4. **Adobe Premiere Pro ➜ Kdenlive or DaVinci Resolve**
   - Kdenlive is a user-friendly and capable editor for most users. DaVinci Resolve (has a native Linux version) is more advanced and professional, but hardware requirements are higher.
5. **Audacity works on both Windows and Linux for audio editing!**
6. **WinRAR / 7-Zip ➜ PeaZip or Archive Manager (default in most desktop environments)**
   - PeaZip is a full-featured archive utility supporting a wide range of formats. The default Archive Manager has worked perfectly fine for my needs as well.
7. **Microsoft Outlook ➜ Thunderbird**
   - Thunderbird, by Mozilla, is a mature and extensible email client with calendar and add-on support.
8. **Microsoft Teams / Skype ➜ Teams (web app) / Element / Discord**
   - Many messaging services now have Linux clients or web versions. I use Discord on my Linux computer, and most other messaging clients that don't run on Linux have a web version directly in your browser you can use.
9. **Windows Defender ➜ Not typically needed**
   -  Linux is much less prone to viruses due to its architecture and permission system. Tools like ClamAV exist but are rarely needed for desktop use.
10. **Windows File Explorer ➜ Dolphin (KDE), Nautilus (GNOME), or Thunar (XFCE)**
    - What do all those acronyms mean!? They're desktop environments. Think of how Windows 10 looks, with the toolbar at the bottom, apps on the desktop, and compare it to macOS, with apps on the bottom center in a "dock". They have slight differences in appearance and sometimes performance.
    - The user-friendly distros I will recommend here in a bit come with its own file manager comparable to File Explorer.
11. **Remote Desktop Connection ➜ Remmina or KRDC**
    - Remmina supports RDP, VNC, SSH, and more. I personally use Remmina a lot for a computer of mine located at a different location.
12. **Task Manager ➜ System Monitor (GNOME), KSysGuard (KDE), or htop (terminal)**
    - Usually comes with its own version of Task Manager where you can check what is using up the most resources on your computer. htop is a powerful, interactive terminal-based process viewer if you feel like trying out Terminal.
13. **Notepad++ ➜ Geany, Gedit, or VS Code**
    - If you are a developer, you should probably be using something like VSCode already, which runs natively on Linux.

Wondering about all the other things? Most everything else is provided already with your distro. Drawing, Settings, Text Editor, Update Manager, Driver Manager, Software Manager, Timeshift (similar to Time Machine for macOS), Sticky Notes, and more will likely already be included. More apps you want to download are usually provided in a sort of "App Store", vetted and ready to download with one click. This includes popular apps like Spotify and Blender.

## Okay, how do I install Linux and use it?

Your first order of business is choosing a distro. There are quite a few out there, so I will provide a concise, beginner friendly list of only three.

1. **[Linux Mint](https://linuxmint.com/)** is widely considered the most beginner-friendly option available. It comes with extensive hardware driver support built-in, including proprietary drivers for graphics cards and wireless adapters that are automatically detected and installed. Software management is handled through both a user-friendly Software Manager (graphical app store) and the traditional APT package manager. The Cinnamon desktop environment feels very familiar to Windows users, with a taskbar, start menu, and system tray in expected locations. Mint typically requires minimal tweaking after installation, though you might want to install additional codecs for media playback, which the system will prompt you about for an easy install.
2. **[Ubuntu](https://ubuntu.com/)** offers robust out-of-the-box hardware support and automatically handles most drivers, including offering easy installation of proprietary graphics drivers through its Additional Drivers tool. Software can be installed via the Ubuntu Software Center (snap packages) or APT, giving you multiple options. The GNOME desktop environment is quite different from both Windows and macOS, featuring a dock-like launcher and unique workflow, though it's intuitive once you adjust. Ubuntu generally needs little post-installation tweaking, but some users prefer to install restricted extras for multimedia codecs and enable additional repositories for broader software selection.
3. **[Pop!_OS](https://system76.com/pop/)** excels at hardware compatibility, particularly for gaming systems, with NVIDIA drivers pre-installed on the appropriate ISO and excellent support for newer hardware. Software management works through the Pop!_Shop and APT, with Flatpak support included. The customized GNOME interface incorporates some unique productivity features like automatic window tiling, creating something that's neither quite Windows nor macOS but remains approachable. Pop!_OS is designed to work immediately after installation with minimal configuration needed, though you might want to explore its advanced tiling features and customize keyboard shortcuts to fully utilize its productivity enhancements.

Read through each one's website, check out some reviews on YouTube or blog posts (look at the bottom of this post for resources), and then we can continue to download one. Don't worry, you can download each one and try it out on your computer without affecting anything on your current operating system, but I still recommend making a backup of your data no matter what.

The download process varies for each one, but is mostly similar, so I will go through it using Linux Mint as an example. Linux Mint is what I use for my personal computer and I definitely recommend it.

The key thing to understand is that you're essentially creating a special USB drive that can start up a computer and run Linux Mint without touching your existing system. The "live session" part is really the magic here - it lets you test drive Linux Mint completely risk-free. You can browse the web, check email, play music, and see how everything works on your specific hardware before making any permanent changes.

Think of it like test driving a car before buying it. The USB drive becomes a temporary operating system that runs entirely from memory, so when you restart your computer, everything goes back to exactly how it was before. The actual installation step is optional and permanent. Most people are surprised by how well modern Linux distributions work with their hardware right out of the box, but it's always better to verify this before committing to an installation.

### What You'll Need
Before starting, gather these items:

- A USB flash drive (8GB or larger)
- A computer with internet access
- About 2-3 hours of free time
- Your important files backed up (just in case)

### Step 1: Download Linux Mint

Visit the [official Linux Mint website (linuxmint.com)](https://www.linuxmint.com/edition.php?id=319) and download the latest version. Choose the "Cinnamon" edition if you're unsure, since it's the most Windows-like. The file you download will be called an "ISO file" and will be several gigabytes in size, so it might take a while to download. Check out [Linux Mint's official installation guide](https://linuxmint-installation-guide.readthedocs.io/en/latest/) for some extra help.

### Step 2: Create Your Installation USB Drive

On Windows and Mac:
1. Download ["balenaEtcher" from balena.io/etcher](https://etcher.balena.io/#download-etcher)
2. Insert your USB drive into the computer
3. Open Etcher, select your ISO file, select your USB drive, then click "Flash." Make sure you choose the correct USB drive, because everything on it will be erased!

You can also use [Rufus for Windows](https://rufus.ie/en/), but I have found Etcher to do the job very well for both Mac and Windows.

### Step 3: Test Drive Linux Mint (AKA a Live Session)

This is the exciting part - you can try Linux Mint without changing anything on your computer!

1. Restart your computer with the USB drive plugged in
2. Access the boot menu by pressing a key immediately during startup:
   - Most computers: F12, F2, F8, or ESC
   - Some HP computers: F9
   - Some Dell computers: F12
   - The exact key usually appears on screen briefly when you first turn on the computer
3. Select your USB drive from the boot menu (it might be called "USB" or show the brand name of your flash drive)
4. Choose "Start Linux Mint" from the menu that appears

Learn more about [what the Boot Menu is from Lenovo's site](https://www.lenovo.com/us/en/glossary/boot-menu/) and see more details for this step on [Mint's installation guide](https://linuxmint-installation-guide.readthedocs.io/en/latest/boot.html).

After a minute or two, you'll see the Linux Mint desktop. Congratulations! You're now running Linux Mint directly from your USB drive. Everything you see is temporary, when you restart, your computer will go back to normal.

### Step 4: Explore and Test

Take some time to click around and try things out:

1. Open the web browser (Firefox)
2. Check if your Wi-Fi works
3. Test your speakers and microphone
4. Try plugging in a printer or other devices
5. Open some programs from the menu

Everything should work just like a regular computer. If something doesn't work properly during this test, it probably won't work after installation either, at least not without some tweaking. It's worth mentioning that performance may seem slower from the USB drive since it might be a less powerful storage device than your internal HDD or SDD that comes with your computer and which is storing your current operating system and data.

### Step 5: Install Linux Mint (optional)

> Important: This step will replace your current operating system. Make sure you have backups of important files first!
{: .prompt-danger }

If you're happy with how everything works, you can install Linux Mint permanently:

1. Double-click the "Install Linux Mint" icon on the desktop
2. Choose your language and keyboard layout
3. Connect to Wi-Fi if you haven't already
4. Choose installation type:
    - "Erase disk and install Linux Mint" - This replaces your current system entirely (most common choice)
    - "Install Linux Mint alongside [current OS]" - This lets you choose between systems when you start up (dual boot)
    - "Something else" - Advanced option for custom setups
5. Select your time zone and create a user account
6. Wait for installation (usually 15-30 minutes)
7. Restart when prompted and remove the USB drive

### What Happens After Installation

When your computer starts up, you'll see the Linux Mint login screen. Enter the username and password you created during installation. Your computer now runs Linux Mint instead of (or alongside, depending on if you chose to dual boot) your previous operating system. All your programs, settings, and files from the live session are gone - you're starting fresh with a clean installation.

### Getting Started Tips

- **Update your system:** The first thing to do is open "Update Manager" and install any available updates
- **Install software:** Use the "Software Manager" to find and install programs. It works like an app store, like the Microsoft Store or Apple App Store
- **Explore the menu:** Click the menu button in the bottom-left corner to see all available programs
- **Customize:** Right-click on the desktop or taskbar to change how things look and behave

If you don't see a program you need in the Software Manager, you will probably have to visit the website for that application. For example, Discord's download page has a download button for Linux. A "deb" or "tar.gz" file is like Window's .exe file or Mac's .pkg/.dmg installation file.

### If Something Goes Wrong

Don't panic! Here are common solutions:

- **Can't boot from USB:** Try a different USB port, check that you pressed the right key for boot menu, or look up your specific computer model's boot key online
- **Computer won't start after installation:** This is rare, but you can usually fix it by booting from the USB again and running "Boot Repair"
- **Missing drivers:** Linux Mint includes a "Driver Manager" that can install additional drivers if needed

The Linux Mint community is very helpful for beginners, so make sure to check out [forums.linuxmint.com](https://forums.linuxmint.com/) for an online community, or call/visit a local computer repair shop to see if they can assist with Linux installations.

### Recommended Resources

**Official Documentation & Guides**
- [The Linux Documentation Project (TLDP)](https://tldp.org/) - Comprehensive guides, HOWTOs, and FAQs covering everything from basics to advanced topics
- [Arch Wiki](https://wiki.archlinux.org/title/Main_page) - Even if you don't use Arch Linux, their wiki is incredibly detailed and applies to most distributions
- [Ubuntu Documentation](https://help.ubuntu.com/) - Well-organized official docs that cover common scenarios
- [ExplainShell.com](https://explainshell.com/) - Explains any shell command in detail

**Books (Available Online)**
- ["The Linux Command Line" by William Shotts](https://linuxcommand.org/tlcl.php) - Available free online, excellent for beginners
- ["Linux From Scratch"](https://www.linuxfromscratch.org/) - Teaches you Linux by building your own distribution from source
- ["Advanced Bash-Scripting Guide"](https://tldp.org/LDP/abs/html/) - Comprehensive resource for shell scripting [[PDF](https://carma.astro.umd.edu/nemo/pitp/papers/abs-guide.pdf)]

**Interactive Learning**
- [OverTheWire Wargames](https://overthewire.org/wargames/) - Hands-on security challenges that teach Linux skills
- [Linux Survival](https://linuxsurvival.com/) - Interactive command line tutorial

**Community Resources**
- [Stack Overflow](https://stackoverflow.com) and [Unix & Linux Stack Exchange](https://unix.stackexchange.com/) - For specific troubleshooting questions
- [r/linux4noobs](https://www.reddit.com/r/linux4noobs/) and [r/linuxquestions](https://www.reddit.com/r/linuxquestions/) on Reddit - Beginner-friendly communities
- Linux.org forums - Active community for all skill levels

**YouTube Channels**
- [The Linux Experiment](https://www.youtube.com/@TheLinuxEXP) - Current Linux news and tutorials
- [LearnLinuxTV](https://www.youtube.com/@LearnLinuxTV) - Systematic Linux education content

The key is to start with hands-on practice in a virtual machine or spare computer, and don't be afraid to break things. That's often how you learn the most about fixing them.