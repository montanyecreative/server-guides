# Table of Contents
- [Trash Guides](#trash-guides)
- [Applications](#applications)
- [Plex](#plex)
    - [Getting Started](#getting-started)
    - [Client Settings](#client-settings)
- [DVDs](#dvds)
    - [Use makemkv](#use-makemkv)
    - [To edit/rename the resulting files](#to-editrename-the-resulting-files)
    - [For inspecting video/audio files](#for-inspecting-videoaudio-files)
- [Hardware](#hardware)
    - [Supporting Plex Transcoding](#supporting-plex-transcoding)
    - [AV1 Decoding Support](#av1-decoding-support)
    - [Playing UHD Blu-ray](#playing-uhd-blu-ray)
    - [Remote Power Switch](#remote-power-switch)
    - [4K/HDR/h264/h265/VP9 under $500](#4khdrh264h265vp9-under-500)
- [Notes](#notes)
    - [Current Setup](#current-setup)
        - [PC Specs](#pc-specs)
        - [Games](#games)
        - [Photos](#photos)
        - [Music](#music)
        - [Movies](#movies)

# Trash Guides

https://trash-guides.info/

# Applications

https://wiki.servarr.com/

# Plex

https://trash-guides.info/Plex/

### Getting Started

https://trash-guides.info/Plex/Tips/Plex-media-server/

### Client Settings

https://trash-guides.info/Plex/Tips/Optimal-plex-client-settings/

# DVDs

I’d recommended using sonarr + trashguides of which I believe I linked you before to organize / name the episodes

### Use makemkv

You don’t actually need to buy MakeMKV. You get full access for 30 days, after which you can uninstall and reinstall for another 30 days.
https://www.makemkv.com

### To edit/rename the resulting files

https://mkvtoolnix.download

### For inspecting video/audio files

Adds a right click dialog
https://mediaarea.net/en/MediaInfo

# Hardware

https://r-htpc.github.io/wiki/components

### Supporting Plex Transcoding

https://support.plex.tv/articles/200250377-transcoding-media/

TLDR: When a client, i.e. a phone requests a certain file from the server but it's a file type normally unplayable on that device, the plex server will take that file and automatically convert it to a playable file type for the device. More powerful CPU = better/faster

CPU REQ: Intel >= i3/i5/i7-7xxx iGPU

### AV1 Decoding Support

Greater than or equal to: Intel i3/i5/i7-11xxx iGPU

### Playing UHD Blu-ray

To play UHD Blu-ray from a Plex server, a specific setting is required found in a small portion of Intel CPUs and motherboards called SGX. Building a computer that supports SGX in 2025 is challenging because the motherboards can no longer be found new.

Supported CPUs = i3/5/7/9-7xxx-10xxx(Comet Lake) Gen iGPU ONLY.

List of motherboards that support SGX

MOTHERBOARD | FORM | USERS | VENDOR | SOURCES/NOTES
--- | --- | --- | --- |---
EVGA H370 Stinger | M-ITX | YES (22a) | YES | CL, SGX
ASRock Fatal1ty Z170 Gaming-ITX/ac | M-ITX | YES (1a) | YES (1b) | SL/KL, SGX, MCDP2800 (19), blu-ray forum
ASRock Fatal1ty Z270 Gaming-ITX/ac | M-ITX | YES (2a) | YES (2b) |SL/KL, SGX, MCDP2800 (19), Asrock HDCP 2.2 key DL
ASRock Fatal1ty Z370 Gaming-ITX/ac | M-ITX | YES (24a) | YES (24b) | CL, SGX
ASRock Z490 Phantom Gaming-ITX/TB3 | M-ITX | YES (25a) | YES (5b) | CML/CML+/RL, SGX, HDMI 2.0 (5c), TB3, or DP 1.4 w/DP->HDMI adapter (6b)
Asus Z270-WS | ATX | YES (4a) | YES (4b) | SL/KL, SGX
Asus Z170-DELUXE | ATX | NA | YES (3b) | SL/KL, SGX, blu-ray forum
Asus Z170-PREMIUM | ATX | NA | YES (3b) | SL/KL, SGX
Asus ROG STRIX Z390-I GAMING | M-ITX | YES (7a) | YES | CL/CL+, SGX, ParadeTech PS175 (20)
Asus Rog Strix Z490-I Gaming | M-ITX | YES (25a) | YES (5b) | CML/RL, SGX, HDMI 2.0 (5c) or DP 1.4 w/DP->HDMI adapter (6b)
GigaByte Aorus GA-Z270X-Gaming 8 | ATX | YES (11a) | YES | SL/KL, SGX, MCDP2800 (19)
GigaByte Aorus GA-Z270X-Gaming 9 | E-ATX | YES (12a) | YES | SL/KL, SGX, MCDP2800 (19)
GigaByte Z390 I Aorus Pro Wi-Fi | M-ITX | YES (25a) | YES | CL/CL+, SGX
GigaByte Z370N-WIFI | M-ITX | YES (12a) | YES | CL, SGX, MCDP2800 (19)
GigaByte H370N-WIFI | M-ITX | YES (12a) | YES | CL, SGX, MCDP2800BC (19)
Gigabyte Z490I Aorus Ultra | M-ITX | YES (26a) | YES (5b) | CML/RL, SGX, HDMI 2.0 (5c) or DP 1.4 w/DP->HDMI adapter (6b). PS175 chip (20)
Gigabyte H470I AORUS Pro AX | M-ITX | YES (25a) | YES (5b) | CML/RL, SGX, HDMI 2.0 (5c) or DP 1.4 w/DP->HDMI adapter (6b). PS175 chip (20)
GigaByte GA-IMB310TN | Thin M-ITX | YES (23a) | YES | CL, SGX, H310
Supermicro C7Z270 PG | ATX | NA | YES | SL/KL, SGX, ParadeTech PS175 (20), blu-ray forum
Supermicro C7Z270 CG | ATX | YES (14a) | YES | SL/KL, SGX, ParadeTech PS175 (20), blu-ray forum
Supermicro C9Z390-CG-IW | M-ITX | NA | YES | CL/CL+, SGX, ParadeTech PS175 (20)
Supermicro C9Z490-PGW / C9Z490-PG | ATX | NA | YES (5b) | CML/RL, SGX, ParadeTech PS175 (20). HDMI 2.0 (5c), DP 1.4, w/DP->HDMI adapter (6b)
Biostar Z270GT9	| ATX | YES (15a) | YES (15b) | SL/KL, SGX, MCDP2800-CC (19), blu-ray forum
Biostar Z270GT8 | ATX | YES (16a) | YES (15b) | SL/KL, SGX, MCDP2800-CC (19), blu-ray forum
EVGA Z370 Classified K | ATX | YES (21a) | YES	| CL, SGX

### Remote Power Switch

This piece of kit can supposedly turn on computer remotely. Worth looking into:

-   https://www.aliexpress.us/item/3256808045747846.html
-   https://www.aliexpress.us/item/3256808023447612.html

Product to research: https://www.aliexpress.us/item/3256807165859143.html?gatewayAdapt=glo2usa4itemAdapt

### 4K/HDR/h264/h265/VP9 under $500

Also runs 4k@60hz and has newer AV1 media decoding.

https://www.newegg.com/dell-vostro-3910-student-home-office/p/1VK-0001-6EVJ7?Item=9SIAA0SJT93276

# Notes

What am I trying to host?

-   Games - return to moria, maybe minecraft
-   Photos - all digitized photos that I have
-   Music - burn CDs, all digital files, digitize vinyl eventually
-   Movies - burn dvds and blurays, digitize VHS, any digital files

## Current Setup

### PC Specs

-   https://pcpartpicker.com/list/4cxMFZ
-   Windows 10 Home

### Games

-   Return to Moria
-   Aloft

### Photos

None

### Music

None

### Movies

None
