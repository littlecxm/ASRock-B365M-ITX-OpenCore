# ASRock-B365M-ITX-OpenCore

ASRock-B365M-ITX/ac OpenCore Bootloader

---

## Hardware

- CPU:Intel i5-9400
- MB:ASRock B365M-ITX/ac Mini ITX LGA1151 Motherboard
  - Chipset: B365
  - LAN:Intel
  - WLAN:Intel 3168NGW(Need replace to BCM DW1820A-08PKF4)
  - HDAudio:
- RAM:HyperX Fury 16GB (HX424C15FB/16)

## Tutorial

- [华擎 Asrock B365M-ITX/ac macOS Catalina 完美黑苹果 OC/Clover 双版本](https://www.chenweikang.top/?p=846)
- [OpenCore Desktop Guide](https://dortania.github.io/OpenCore-Desktop-Guide/)

## Based On

- [Good0007/B365ITX-Hackintosh-OC](https://github.com/Good0007/B365ITX-Hackintosh-OC/releases)

## Requirement

### Drivers

- OpenCore from [acidanthera/OpenCorePkg](https://github.com/acidanthera/OpenCorePkg)
- HFSPlus.efi from [acidanthera/OcBinaryData](https://github.com/acidanthera/OcBinaryData)

### Kexts

1. [Lilu](https://github.com/acidanthera/lilu/releases)
2. [VirtualSMC](https://github.com/acidanthera/virtualsmc/releases)
3. SMCProcessor (Include on VirtualSMC)
4. SMCSuperIO (Include on VirtualSMC)
5. [WhateverGreen](https://github.com/acidanthera/WhateverGreen/releases)
6. [AppleALC](https://github.com/acidanthera/applealc/releases)
7. [IntelMausi](https://github.com/acidanthera/IntelMausi/releases)
8. [AirportBrcmFixup](https://github.com/acidanthera/airportbrcmfixup/releases)
9. BrcmFirmwareData from [BrcmPatchRAM](https://github.com/acidanthera/BrcmPatchRAM/releases)
10. BrcmPatchRAM3 from [BrcmPatchRAM](https://github.com/acidanthera/BrcmPatchRAM/releases) (on macos 10.15.xx)
11. BrcmBluetoothInjector from [BrcmPatchRAM](https://github.com/acidanthera/BrcmPatchRAM/releases)
12. [NVMeFix](https://github.com/acidanthera/NVMeFix/releases)
13. [RehabMan/OS-X-USB-Inject-All](https://bitbucket.org/RehabMan/os-x-usb-inject-all/downloads)
14. USBPorts Customed by [Hackintool](https://github.com/headkaze/Hackintool/releases)
15. USBPower Customed by [Hackintool](https://github.com/headkaze/Hackintool/releases)

## Tools

- [gibMacOS](https://github.com/corpnewt/gibMacOS) for make macos Recovery USBDisk
- [WEPE](http://www.wepe.com.cn) (for embedded OpenCore EFI)

## BIOS Configure

- CPU
  - CFG Lock: On -> off
- USB
  - XHCI Hand-Off : Off -> On
- Boot
  - CSM : On -> Off
