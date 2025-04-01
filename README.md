# ASRock Z890I Nova WiFi EFI
EFI for the ASRock Z890I Nova WiFi with OpenCore 1.0.4.

* **BIOS Version:** 2.26
* **macOS Version:** Sequoia 15.3.2
* **Processor:** Core Ultra 7 265

## Kexts
* AppleALC.kext
* BlueToolFixup.kext
* IntelBluetoothFirmware.kext
* IntelBTPatcher.kext
* itlwm.kext
* Lilu.kext
* RestrictEvents.kext
* RtWlanU.kext
* RtWlanU1827.kext
* SMCProcessor.kext
* SMCSuperIO.kext
* USBToolBox.kext
* UTBMap.kext
* VirtualSMC.kext
* WhateverGreen.kext

## Notes
* Disable VT-d for first boot. Enable afterwards and subsequent boots should still work fine.
* Installed from a USB 2 thumb drive since boot attempts from a USB 3 drive got stuck.
* Using a TP-Link TL-WN823N USB Wi-Fi adapter for Wi-Fi connectivity. See https://github.com/chris1111/Wireless-USB-OC-Big-Sur-Adapter/ for driver installation.
* Using a generic USB-to-Ethernet adapter for Ethernet connectivity.


## Current Status
* Boots.
* Audio works.
* Bluetooth works.
* Intel BE200 Wi-Fi NOT working.
* Realtek RTL8126 5G Ethernet NOT working.

![About](https://github.com/user-attachments/assets/38cecbb8-f030-4624-92df-15f2d6b59619)

![Geekbench - no perf optimisations](https://github.com/user-attachments/assets/e10c087a-4b0e-4e16-9bac-e96fa8511059)

## USB Port Mapping
Ports mapped using USBToolBox on Windows.

## BIOS Settings

### Enabled
| Setting                        | Where?                           |
| ------------------------------ | -------------------------------- |
| Re-Size BAR Support            | Advanced \ Chipset Configuration |
| VT-d                           | Advanced \ Chipset Configuration |
| Intel Virtualization Techology | Advanced \ CPU Configuration     |
| XHCI Hand-off                  | Advanced \ USB Configuration     |


### Disabled
| Setting              | Where?                           |
| -------------------- | -------------------------------- |
| Fast Boot            | Boot                             |
| IGPU Multi-Monitor   | Advanced \ Chipset Configuration |
| Intel Platform Trust | Security                         |
| Secure Boot          | Security                         |

## Hardware
| Component         | Model                                           |
| ----------------- | ----------------------------------------------- |
| CPU               | Intel Core Ultra 7 265                          |
| Motherboard       | ASRock Z890I Nova WiFi                          |
| RAM               | 96GB (2 x 48GB) G.SKILL Ripjaws S5 @ 6400MT/s   |
| GPU               | ASRock AMD Radeon RX 6600 XT Challenger ITX 8GB |
| OS Drive          | WD_BLACK SN850X 1TB                             |
| Audio             | Realtek ALC4080                                 |
| Wi-Fi / Bluetooth | Intel Wi-Fi 7 BE200 (Wi-Fi not working)         |


## Disclaimer
By using this EFI, you acknowledge it is provided "as is" without warranties of any kind. The developers and associated parties are not liable for any damage to equipment, data loss, or other consequences arising from its use. It is your responsibility to ensure the EFI does not harm your system and to back up data before use. By using this EFI, you agree to use it at your own risk.
