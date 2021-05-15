# Instroduce
## Laptop Dell Inspiron 7447

Detail Spesification
* Processor : Intel Core i5 4210H @2.9Ghz
* IGPU : Intel HD Graphics 4600
* GPU Discrette : Nvidia GTX 850M
* RAM : 8GB DDR3L PC12800/Bus 1600Mhz (4GB + 4GB)
* Storage : SSD Samsung 850 EVO 500 GB + HDD 500GB
* Audio Codec : Realtek ALC255
* Wifi : Intel Wireless Dual Brand AC 3160 + Bluetooth
* Ethernet : Realtek RTL8111 Gigabit Ethernet
* Touchpad : PS2 Interface (Synaptics)
* Screen Size : 14" HD
* Screen Resolution : 1366x768
* OS : Windows 10 Pro is activated
* Boot Mode : UEFI + GPT
* Bootloader: Clover v5.1 r5xxx release and lastest
* OS version: macOS Catalina 10.15.x and lastest

## Working
* CPU Power Management
* Sleep/Wake
* Restart/Shutdown
* Internal Speaker, Audio Digital Out, Headphone and Microphone
* Audio Realtek AC255 (layout-id = 20)
* Intel WiFi AC-3160
* Disable dGPU (card Nvidia GTX)
* Brightness + Fn up/down
* All USB Port
* Trackpad
* Keyboard Backlist

Not working
* Nvidia Card (Switchable Graphics is not supported Hackintosh)
* Bluetooth (Intel Bluetooth is not supported)
* Etc

# Installing
* Copy EFI directory for Clover
* Download [Clover v5.1 release](https://github.com/CloverHackyColor/CloverBootloader/releases)

## Intel WiFi Driver for Hackintosh

* Only kext Big Sur - [My kext for WiFi](https://github.com/kwangle912/AirportItlwm-for-Hackintosh): Kext to /EFI/Clover/Kext/Other
* Only kext Catalina - Disable SIP & install AirportItlwm into /Library/Extensions "With Hackintool" & rebuild kext cache then reboot (use AirportItlwm Catalina and install [Hackintool.app](https://github.com/headkaze/Hackintool/releases))

## Supported Intel WiFi Cards by itlwm
- 2000: `Supported`
- 3xxx: `AC 3160`, `AC 3165`, `AC 3168`
- 4xxx: `AC 4165`
- 7xxx: `AC 7260`, `AC 7265`
- 8xxx: `AC 8260`
- 9xxx：`AC 9260`,`AC 9461`, `AC 9462`, `AC 9560`
- 22000：`ax200`, `ax201`, `AC 9462`
- [Supported Devices](https://openintelwireless.github.io/itlwm/Compat.html)
- Link download [AirportItlwm.kext](https://github.com/kwangle912/AirportItlwm-for-Hackintosh)

Download [HeliPort.app](https://github.com/OpenIntelWireless/HeliPort/releases)
* Install Heliport.dmg to Applications and open Heliport.app (No reboot)
* Check on Heliport with Preferences "Open launch At Login" ✅
* Note: If you want to reset the assignment to en0, 
just delete ❌:/Library/Preferences/SystemConfiguration/NetworkInterfaces.plist and reboot. Enjoy 🎉
