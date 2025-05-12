# EFI-RYZEN-B550-RX6600

:information_source: **The current version is fully macOS Monterey to macOS Sequoia compatible.**
OpenCore, drivers, and kexts are always up to date! (as soon as possible)

<br/>

## Current Status
[![OpenCore](https://img.shields.io/badge/OpenCore-1.0.2-lightblue.svg)](https://github.com/acidanthera/OpenCorePkg)
[![macOS](https://img.shields.io/badge/macOS-15.0.1-F09337.svg)](https://www.apple.com/macos/ventura)

## :warning: Disclaimer


This repository contains ONLY my complete EFI configuration based on personal experiments with my specific hardware. This is NOT a guide and should NOT be used as such. Before doing anything, please refer to the official [Dortania guide](https://dortania.github.io/getting-started/). This OpenCore configuration is optimized for my specific hardware. Use it only as a reference or if you have exactly the same or very similar hardware. I am NOT responsible for any damage caused by misuse of this configuration.

## :computer: Hardware:

| **Category** | **Component**                                                                    |
| ------------ | -------------------------------------------------------------------------------- |
| **CPU**      | 3,5 GHz AMD Ryzen 5 5600 6-Core Processor                                        |
| **GPU**      | ASROCK Challenger - AMD Radeon RX 6600 8 GB Challenger 8GB                       |
| **RAM**      | 16GB GLOWAY DDR4 3200MHZ (XMP)                                                   |
| **CHIPSET**  | ASUS TUF GAMING B550-PLUS [ASUS](https://www.asus.com/motherboards-components/motherboards/tuf-gaming/tuf-gaming-b550-plus/) |
| **SSD**      | 120GB ADATA SATA                                                                 |
| **Wi-Fi/BT** | Intel AX210                                                                      |
| **Ethernet** | Realtek RTL8125B 2.5Gb Ethernet                                                  |
| **Audio**    | Realtek ALC S1200A                                                               |

## :white_check_mark: Working:

- [x] CPU power management.
- [x] Graphics acceleration.
- [x] Keyboard & Mouse
- [x] Wi-Fi.
- [x] USB ports.
- [x] HDMI video & audio output.
- [x] Ethernet.
- [x] Audio (Internal speakers, 3.5mm headphone jack).
- [x] Internal microphone.
- [x] VGA WebCam.
- [x] iCloud & App Store.
- [x] iMessage & FaceTime.

## :x: Not working:
- [ ] Bluetooth. ? i don't need it i didn't try to fix it
- [ ] AirDrop. ? probably related to Bluetooth, i don't need it i didn't try to fix it

## :closed_lock_with_key: SMBIOS

You will need to generate your own SMBIOS and configure, since is required to fully work with macOS. As per this [guide](https://dortania.github.io/OpenCore-Install-Guide/AMD/zen.html#platforminfo) you can use the following SMBIOS: iMacPro1,1 or MacPro7,1. Note that if your hardware is different for the one mentioned [here](#computer-hardware) you have tho choose an appropriate SMBIOS, more details in the [guide](https://dortania.github.io/OpenCore-Install-Guide/AMD/zen.html).

Use [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS) to generate your own unique SMBIOS and then copy each parametter following path (recomended to follow the guide above):

- Config.plist -> PlatformInfo -> Generic

## BIOS setup:

IMPORTANT: Need to **enable** Above 4G Decoding and set Resize BAR to Auto on BIOS or will not work!
If you don't have this on your BIOS you will need to adjust the config.plist, refer to [AMD bios settings](https://dortania.github.io/OpenCore-Install-Guide/AMD/zen.html#amd-bios-settings) and [boot-args](https://dortania.github.io/OpenCore-Install-Guide/AMD/zen.html#nvram)


## Credits:

https://github.com/gabrielcasag/EFI-RYZEN-5600-B550-RX6600
[**Gabriel Gasperi Casagrande**](https://github.com/gabrielcasag/EFI-RYZEN-5600-B550-RX6600)

[**Gabriel Luchina**](https://luchina.com.br)

[**AMD-OSX**](https://github.com/AMD-OSX/AMD_Vanilla)

[**Acidanthera**](https://github.com/acidanthera)

[**Dortania**](https://dortania.github.io/getting-started/)

[**Apple**](http://apple.com/)
