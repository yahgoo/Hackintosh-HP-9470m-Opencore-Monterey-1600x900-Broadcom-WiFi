## HP 9470m Opencore Monterey 1600x900 Broadcom WiFi
* Opencore EFI for HP Elitebook 9470m 1600x900 Broadcom WiFi running Monterey 12.2.1
* Bluetooth fixed with BlueToolFixup.kext and enable only AirPortBrcmNIC_Injector.kext
* ECEnabler.kext to enable Battery Indicator. Please ignore the BTST and BTIF errors during macos installation as ECEnabler.kext is not yet loaded.
* HD4000 patched with OC 0.7.9 Post Install Root Patch  
* Rename Monterey System Volume name with Disk Utility. According to @miliuco, the workaround is to install Intel Power Gadget in order to update both the OC boot menu entry and the preboot volume with new name.

## Credits  
Opencore  
hackintosh107  
InsanelyMac - Miliuco  
1Revenger  
Robbish  
Sirsasana  

## Changes
06042022
- Updated to MacOS Monterey 12.2.1
- Updated to OC 0.7.9 and latest kexts like VirtualSMC
- SMBIOS iMac17,1 in order for OC 0.7.3 and above to boot and bypass the prompt that “a required firmware update could not be installed” during installation. 

![Screenshot](https://github.com/yahgoo/Hackintosh-HP-9470m-Opencore-Monterey-1600x900-Broadcom-WiFi/blob/main/img/HP9470m%20Monterey%2012-2-1%20iPad%20Mini%206%20Purple.png)

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
* OpenCore: 0.7.9
* macOS: Monterey 12.2.1

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

## Set bios settings as follows:
Advanced tab:  
Boot options:  
- Fast Boot = Disabled
- Network (PXE) Boot = Disabled  
Secure Boot Configuration:
- "Legacy Support Enable and Secure Boot Disable"  
System Options:  
- Virtualization Technology (VTx) = Disabled (recommended, Enable also worked)
- Virtualization Technology for Direct I/O (VTd) = Disabled (recommended, Enable also worked)  
Built-In Device Options:  
- Wake On LAN = Disabled
- Video memory size = 64 MB
- LAN/WLAN Auto Switching = Disabled
- Fingerprint Device = Disabled  
Power Management Options:  
- Extended Idle Power States = Disabled
- Deep sleep = You can keep this enabled
- Wake when Lid is Opened = Enabled
- Wake on USB = Disabled
