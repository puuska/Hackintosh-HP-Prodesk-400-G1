# HP ProDesk 400 G1 - Mojave Hackintosh
## Configuration

| Specifications | Details                                                  |
| ------------------- | ------------------------------------------- |
| Computer model      | HP Prodesk 400 G1 SFF      					|
| Processor           | Intel Core i3-4130 Processor    		    |
| Integrated Graphics | Intel HD Graphics 4400/4600                 |
| Sound Card          | Realtek ALC221 (layout-id:11/15)            |
| Ethernet		      | Realtek RTL8168G                        		|

![hackintosh desktop](https://i.imgur.com/rbMhHpv.png)
## Improvements
- Use https://github.com/Piker-Alpha/ssdtPRGen.sh to optimize CPU power management
- After installation, open terminal and use the command `sudo spctl --master-disable` to allow apps from unidentified developers
- ACPI sleep is working. You can wake up the computer using the keyboard. If any issues with sleep arise, open terminal and use the command `sudo pmset -a standby 0` to resolve issues with waking up.
## Installation

### First-time installation
First of all, go to the UEFI settings and disable the serial port. Upgrade the BIOS to the newest possible version (currently the newest version is version no. [00.02.56, Rev.A](https://ftp.hp.com/pub/softpaq/sp96001-96500/sp96015.exe) which was released on the 30th of April 2019)
To install it, download the Olarila distro image from their forums, burn it to a USB Stick with Etcher (under Linux) or Win32DiskImager (under Windows) and replace the Clover folder entirely with the folder from this repo.

### Issues
- VGA Display output isn't working
- If you are going to install Catalina instead of Mojave, be aware that the TV app and Sidecar don't work.
- I'm not sure about 4K, but according to Donw35 from the InsanelyMac forums it doesn't work.
- While installing, make sure your USB Stick, keyboard and mouse are attached to USB2.0 ports instead of USB3.0. 3.0 ports do work fine in the system itself, though.
## A reward

The entirety of this project is available free of charge, but you can give me a small reward (if you want to).

[PayPal](https://paypal.me/puuska)

## Credits
- Very big thanks to [Donw35](https://www.insanelymac.com/forum/profile/150555-donw35/) from the InsanelyMac forums for his EliteDesk 800 G1 Tutorial that really helped me with creating the EFI for my ProDesk 400 G1;
- thanks to [Acidanthera](https://github.com/acidanthera) for providing [AppleALC](https://github.com/acidanthera/AppleALC), [VirtualSMC](https://github.com/acidanthera/VirtualSMC), [Lilu](https://github.com/acidanthera/Lilu) and  [WhateverGreen](https://github.com/acidanthera/WhateverGreen)
- thanks to [RehabMan](https://github.com/RehabMan) for [OS-X-Realtek-Network](https://github.com/RehabMan/OS-X-Realtek-Network) and [FakePCIID](https://bitbucket.org/RehabMan/os-x-fake-pci-id/downloads/);
- thanks to [corpnewt](https://github.com/corpnewt) for [USBMap](https://github.com/corpnewt/USBMap);
- thanks to [apianti](https://sourceforge.net/u/apianti), [blackosx](https://sourceforge.net/u/blackosx), [blusseau](https://sourceforge.net/u/blusseau), [dmazar](https://sourceforge.net/u/dmazar), and [slice2009](https://sourceforge.net/u/slice2009) for providing [Clover](https://github.com/CloverHackyColor/CloverBootloader);
- thanks to McDonnelltech from [McDonnelltech's Thinkpad X220 Hackintosh Guide](http://x220.mcdonnelltech.com) for his tutorial that has some helpful content for every hackintosh.
