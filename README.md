# HP 9470m Opencore Monterey
* Opencore EFI for HP Elitebook 9470m 1600x900 Broadcom WiFi running Monterey Beta 4  
* Bluetooth fixed with BlueToolFixup.kext and enable only AirPortBrcmNIC_Injector.kext
* ECEnabler.kext to enable Battery Indicator. Please ignore the BTST and BTIF errors during macos installation as ECEnabler.kext is not yet loaded.
* HD4000 patched with patchHD4000
## Credits  
Opencore  
hackintosh107  
chris1111  

![Screenshot](https://github.com/yahgoo/Hackintosh-HP-9470m-Opencore-Monterey/blob/main/img/Screen%20Shot%202021-08-04%20at%204.00.17%20PM.png)

<p align="center">
  <img width="400" height="300" src="/img/HP_9470m.png">
</p>

# Specifications:
* CPU: Intel Core i7-3687U
* GPU: Intel HD Graphics 4000
* Resolution: 1600x900
* Audio: IDT 92HD91BXX
* Wi-Fi: BCM94352HMB
* Bluetooth: Broadcom Bluetooth 4.0
* Ethernet: Intel 82579LM
* Touchpad: Synaptics SMBus TouchPad
* Card reader:
  - JMicron Card Reader
  - Alcor Micro USB Smart Card Reader
* Fingerprint: Synaptics Fingerprint Sensors

# Version: 
* OpenCore: 0.7.2
* macOS: 12.0.1 (Monterey)

# BIOS settings:
* Boot mode: UEFI Native (without CSM)
* SATA mode: AHCI

# Working:
- [x] Intel HD Graphics 4000
- [x] Sleep
- [x] Audio (using AppleALC.kext with layout-id = 13)
- [x] Internal microphone
- [x] External microphone
- [x] Touchpad (with multi gestures)
- [x] Battery indicator
- [x] Ethernet
- [x] Wi-Fi
- [x] Bluetooth
- [x] CPU power management
- [x] Webcam
- [x] USB ports
- [x] Fn function keys
- [ ] Card reader
- [ ] Synaptics Fingerprint Sensors

# SMBIOS:
iMac16,1
