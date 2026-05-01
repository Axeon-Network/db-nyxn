---
layout: custom
title: Windows XP build 3890
permalink: Windows_XP_build_3890
redirect_from:
    - Windows_Server_2003_build_3890
hatnote: "This isn't meant to be here, but I'm not wasting those ~~57~~ 58 screenshots!! -sbf"
---

{% include infoboxes/buildwin.html
buildof='[Windows Server XP](https://betawiki/wiki/Windows_XP)'
family='Windows NT'
buildtag='5.2.3890.x86fre.dnsrv_src.260218-1558'
version='5.2'
build='3890'
lab='dnsrv_src'
arch='x86'
compiled='2026-02-18'
image='WindowsXP3890FirstBoot.png'
image2='Srv2k3_3890FirstBoot.png'
image_caption='First boot (client)'
image2_caption='First boot (server)'
skus='Professional<br>Home Edition<br>Standard Server<br>Enterprise Server<br>Datacenter Server<br>Small Business Server<br>Web Server<br>Preinstallation Environment'
winver='WindowsXP3890Winver.png'
winver2='Srv2k3_3890Winver.png'
prodkey='<i>DDDDD-DDDDD-DDDDD-DDDDD-DDDDD</i> or <i>99999-99999-99999-99999-99999</i>'
%}

**Windows XP build 3890** is a build of [Windows XP](https://betawiki.net/wiki/Windows_XP). It is based on the [OpenXP Project](https://theopenxp.org), which is a modified version of the leaked [Windows Server 2003 RTM](https://betawiki.net/wiki/Windows_Server_2003_build_3790) source code. This build was compiled in evaluation mode and can be installed in the current date.

Other than the build number, lab and compile date, this build is almost identical to the RTM build of Windows Server 2003, with other several bugs and quirks from the OpenXP Project.

This build is available in the Professional, Home Edition, and Server editions, including the Preinstallation Environment.

# Changes
- Unlike the original source, the End-User License Agreement now states that it applies to all the SKUs.
- The background for the Preinstallation Environment has changed from *Ascent* to the Windows Server 2003 branding wallpaper, stating "*Microsoft Windows Preinstallation Environment*" instead of "*Microsoft Windows Server 2003*".

# Bugs and quirks
- While not extensively tested, programs relying on Windows Installer, such as VMware Tools, will fail with a "Setup was unable to upgrade the Windows Installer" error. 
- On the Professional and Home Edition SKUs, the Out of Box Experience (OOBE) will skip most of the pages (including the Welcome page), going straight up to the "Thank you!" page.
- Windows Product Activation is gone from this build, causing all product keys except *DDDDD-DDDDD-DDDDD-DDDDD-DDDDD* and *99999-99999-99999-99999-99999* to fail. This is likely due to the fact that OpenXP (and the original source code leak) had WPA removed for security reasons.
- Opening `msoobe.exe` will open a blank window titled "The Windows oobe.htm". On retail copies of Windows XP, `msoobe.exe` by itself does not open anything.
- Running `msoobe.exe /a` will launch the WPA wizard, but it will state that "Windows is already activated."
- Due to a bug in the start script, the Preinstallation Environment will not display the copyright warning.
