---
layout: post
title: "OmniROM builds updated with KRACK fixes"
date: 2017-10-17 16:00:00 -0500
excerpt: "Nothing ruins your day like a good security vulnerability being released, especially if it affects something you use on a regular basis. If I have just described you, then this one likely could give you a case of heartburn as it affects not just mobile devices, but even your connected toaster."
categories:
- development
tags:
- omni
- security
- news
author:
  display_name: Jeremy
---

Nothing has the potential to ruin your day like a good security vulnerability being released, especially if it affects something you use on a regular basis. If I have just described you, then this one likely could give you a case of heartburn as it affects not just mobile devices, but even your connected toaster.

If you haven't already heard, this new vulnerability involves WiFi and weaknesses in the security protocol WPA2. The name of said vulnerability is KRACKs (__k__ey __r__einstallation __a__tta__cks__) and more information can be found at the official [site](https://www.krackattacks.com/). Luckily Google has responded quickly to [this in Android Oreo](https://android.googlesource.com/platform/external/wpa_supplicant_8/+/master), and we've been working since the announcement and release of the exploit to [backport the patches](https://gerrit.omnirom.org/#/q/status:merged+project:android_external_wpa_supplicant_8+branch:android-7.1+topic:krack_attack) to our official N builds. Thanks to LineageOS for compiling the needed patches.

One of the promises of Omni has always been that we would backport security fixes wherever possible, and that's what we're doing today. Beginning with today's builds, all official OmniROM N builds have the fix included. And regarding O builds, once we're able to bring official Oreo builds to Omni these fixes will be merged unless Google merges these to master first. As needed we will provide updates accordingly.
