# Hackintosh OpenCore configuration for Chinese X79-P3 Motherboard

# Why OpenCore?
OpenCore is FASTER, SAFER that Clover

# What is Working:
  LAN   : Perfect
  SOUND : Perfect
  SLEEP : Works on El Capitan and Sierra 
  NVME  : Perfect
  USB2  : Perfect
  USB3  : Perfect
 
# What is not working:
  SLEEP     : High Sierra, Mojave, Catalina
  Hiberate  : Can't resume.
  
# SSDT/DSDT Patches
 a) HPET
 b) IPIC
 c) Power Management
 d) USB port limit
 e) X79 USB2 Patch
 f) RTC
 g) EC
 h) TMR
 i) CPU package
 
 # Extensions
  1) Lilu.kext (Pathcer)
        a) VirtualSMC.kext (Emulates Mac SMC device)
        b) SMCProccessor.kext (Plugin for virtualsmc)
        c) SMCSuperIO.kext (Plugin for virtualsmc)
        d) WhateverGreen.kext (GPU)
        e) AppleALC.kext   (Sound)
  2) RealtekRTL8111.kext (Ethernet card)
  3) VoodooTSCSync.kext (Sync cpu threads)

# Other Fixes
  Ethernet as built-in (Facetime/iMessage)

## Change log:

2020/06/01: First upload

I'd recommend you read the change logs before updating.

# Hardware Specifications:

## Matherboard: Jingsha X79-P3

OpenCore Version 0.58

Make sure to:

- Disable Serial Port
- Disable VT-d
- Disable USB ECHI
- Enable USB XHCI


## CPU: 3930k

Single CPU

Configured for OC (4,2ghz)
Power Management works (1,2ghz - 4,2ghz)

## Graphic: GTX 750TI

Acceleration works on Sierra and High Sierra.

Needs Nvidia Web driver, if you plan to use amd card remove "nvda_drv" from boot args.


## Lan

Works fine.

## Sound card: Reltek ALC892

Works fine with original AppleHDA, no voodoo kexts :P

# Supported Systems:

- 10.11 El Capitan: Perfect

- 10.12.6 macOS Sierra: Perfect.

- 10.13 macOS High Sierra: Good (Sleep not working on HS due to c600/x79 chipset).

