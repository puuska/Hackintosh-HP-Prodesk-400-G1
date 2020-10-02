# HP ProDesk 400 G1 - Big Sur Hackintosh
## Configuration

| Specifications | Details                                                  |
| ------------------- | ------------------------------------------- |
| Computer model      | HP Prodesk 400 G1 SFF      					|
| Processor           | Intel Core i3-4130 Processor    		    |
| Graphics | NV GT730 GK207                |
| Sound Card          | Realtek ALC221 (layout-id:11/15)            |
| Ethernet		      | Realtek RTL8168G                        		|

![hackintosh desktop](https://i.imgur.com/A97y9aG.png)
## Improvements
- This version was prepared using OpenCore 0.6.1 for MacOS Big Sur.
- SSDT was generated for i3-4130. Use https://github.com/Piker-Alpha/ssdtPRGen.sh to optimize yours CPU power management and then paste it into EFI/OC/ACPI/ssdt.aml
- Everything is working; sleep, USB, sound (dodgy way there!). Even Checkra1n doesn't have any problem with detecting your iPhone in DFU mode.
## Installation

### First-time installation
- First of all, go to the UEFI settings and disable the serial port. Upgrade the BIOS to the newest possible version (currently the newest version is version no. [00.02.56, Rev.A](https://ftp.hp.com/pub/softpaq/sp96001-96500/sp96015.exe) which was released on the 30th of April 2019).
- Copy OpenCore to EFI partition or USB drive. In contrast to Clover, you need to have BOOT\bootx64.efi file.
- Simply put your Big Sur install USB into any port and select Install macOS option in OpenCore.

### Issues
- VGA Display output isn't working
- TV app is working but it is not stable at all. Sidecar is not working.
- VoodooHDA... Can't get AppleALC to work. OpenCore documentation is just a piece of sh*t.


## Credits
- OpenCore with Big Sur support config was created by [bieleckipawel](https://github.com/bieleckipawel);
- thanks to OpenCore developers;
- thanks to [Acidanthera](https://github.com/acidanthera) for providing [VirtualSMC](https://github.com/acidanthera/VirtualSMC), [Lilu](https://github.com/acidanthera/Lilu) and [WhateverGreen](https://github.com/acidanthera/WhateverGreen);
- thanks to [RehabMan](https://github.com/RehabMan) for [OS-X-Realtek-Network](https://github.com/RehabMan/OS-X-Realtek-Network) and [VoodooPS2Controller](https://github.com/RehabMan/OS-X-Voodoo-PS2-Controller);
- thanks to Clover team for providing [VoodooHDA](https://sourceforge.net/p/voodoohda/).
