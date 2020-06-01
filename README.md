## Hackintosh OpenCore configuration for Chinese X79-P3 Motherboard

## Why OpenCore?
OpenCore is FASTER and SAFER than Clover

## Working:
  - LAN
  
  - SOUND
  
  - SLEEP (Works on El Capitan and Sierra)
  
  - NVME
  
  - USB2
  
  - USB3
  
 
## Not working:
  - SLEEP      (High Sierra, Mojave, Catalina)
  - Hiberate   (Can't resume)
  
## SSDT/DSDT Patches
 - HPET
 
 - IPIC
 
 - Power Management
 
 - USB port limit
 
 - X79 USB2 Patch
 
 - RTC
 
 - EC
 
 - TMR
 
 - CPU package
 
 ## Extensions
  1) Lilu.kext (Pathcer)
        a) VirtualSMC.kext (Emulates Mac SMC device)
        
        b) SMCProccessor.kext (Plugin for virtualsmc)
        
        c) SMCSuperIO.kext (Plugin for virtualsmc)
        
        d) WhateverGreen.kext (GPU)
        
        e) AppleALC.kext   (Sound)
        
  2) RealtekRTL8111.kext (Ethernet card)
  
  3) VoodooTSCSync.kext (Sync cpu threads)

## Other Fixes
 - Ethernet as built-in (Facetime/iMessage)

## Change log:

2020/06/01: First upload

I'd recommend you read the change logs before updating.

## Hardware Specifications:

## Motherboard: Jingsha X79-P3

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



## Supported Systems:

- 10.11 El Capitan: Perfect

- 10.12 macOS Sierra: Perfect.

- 10.13 macOS High Sierra: Good (Sleep not working on HS due to c600/x79 chipset).

