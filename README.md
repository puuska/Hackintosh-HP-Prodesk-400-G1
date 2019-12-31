# HP ProDesk 400 G1 Mojave Hackintosh
## Configuration

| Specifications | Detail                                                  |
| ------------------- | ------------------------------------------- |
| Computer model      | HP Prodesk 400 G1 SFF      					|
| Processor           | Intel Core i3-4130 Processor    		    |
| Integrated Graphics | Intel HD Graphics 4400/4600                 |
| Sound Card          | Realtek ALC221 (layout-id:11/15)            |
| Ethernet		      | Realtek RTL8168G                        		|

## Improvements
- Use https://github.com/Piker-Alpha/ssdtPRGen.sh to optimize CPU power management
- After installation, go to terminal and enter `sudo spctl --master-disable` to allow apps from unidentified developers
- Sleep is working, You can wake up using keyboard. If there are any issues with sleep, open terminal and type `sudo pmset -a standby 0` to resolve issues with waking up
## Installation

### First-time installation
First of all, go to UEFI settings and disable serial port. Upgrade BIOS to newest possible version (atm it's 00.02.56 Rev.A released on 30/04/2019 (dd/mm/yyyy) )
To install it, download Olarila image from their forums, burn to USB Stick with Etcher/Win32DiskImager and replace Clover folder with folder from this repo.

## A reward

All the project is made for free, but you can reward me if you want.

[PayPal](https://paypal.me/puuska)

## Credits
- Very big thanks to [Donw35](https://www.insanelymac.com/forum/profile/150555-donw35/) from InsanelyMac forums for EliteDesk 800 G1 Tutorial that really helped me with creating EFI for my ProDesk 400 G1.
- Thanks to [Acidanthera](https://github.com/acidanthera) for providing [AppleALC](https://github.com/acidanthera/AppleALC), [VirtualSMC](https://github.com/acidanthera/VirtualSMC), [Lilu](https://github.com/acidanthera/Lilu) and  [WhateverGreen](https://github.com/acidanthera/WhateverGreen)
- Thanks to [RehabMan](https://github.com/RehabMan) for [OS-X-Realtek-Network](https://github.com/RehabMan/OS-X-Realtek-Network) and [FakePCIID](https://bitbucket.org/RehabMan/os-x-fake-pci-id/downloads/)
- Thanks to [corpnewt](https://github.com/corpnewt) for [USBMap](https://github.com/corpnewt/USBMap)
- Thanks to [apianti](https://sourceforge.net/u/apianti), [blackosx](https://sourceforge.net/u/blackosx), [blusseau](https://sourceforge.net/u/blusseau), [dmazar](https://sourceforge.net/u/dmazar), and [slice2009](https://sourceforge.net/u/slice2009) for providing [Clover](https://github.com/CloverHackyColor/CloverBootloader).
- Thanks to McDonnelltech from [Thinkpad X220](http://x220.mcdonnelltech.com) tutorial that have some helpful content for every hackintosh
