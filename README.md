# ASUS-X550CL-Opencore
Full EFI folder without the recovery images to get Opencore Mojave working on the ASUS X550CL.

# Keep in mind, this is experimental!

## What works:
- Display & brightness
- Sound & microphone
- Battery percentage
- Trackpad
- WiFi (Atheros AR9285)
- Ethernet
- Trackpad gestures

## What is dependent on the user:
- Since the stock Mediatek MT7630e Wi-Fi card that ships with the laptop doesn't work with macOS, I replaced my card with a cheap Atheros AR9285.
- My battery is extremely degraded, so I can't really test the screen on time. I need someone to report to me about that.

## What doesn't work:
- Nvidia GT 710M, due to macOS versions since Mojave not supporting Nvidia cards.
- The stock Wi-Fi card, as mentioned above.
- Wake from sleep
- Your CPU fan might run at full speed sometimes.

How to install:
- Clone the repo and extract the EFI folder into your USB's root directory.
- If you need just the kexts, remember to snapshot your config.plist.
- If you need just the plist, remember to adjust your kexts accordingly.

## Included kexts:
- AirportAtheros40
- AppleHDADisabler
- AtherosWiFiInjector
- ECEnabler
- HibernationFixup (might not be functional sometimes)
- HS80211Family
- Lilu
- RealtekRTL8111
- VirtualSMC and SMC kexts for laptops
- USBInjectAll
- VoodooHDA
- Voodoo trackpad kexts
- WhateverGreen
