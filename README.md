# My Hackintosh

![](img/7.jpg)

My current build runs MacOS Catalina 10.15.5 and is based on a fanless Intel NUC8i5BEK.

## What works, what does not

- ✅ GPU acceleration
- ✅ HDMI audio
- ✅ HDMI and USB-C video at 2560 x 1440 @ 60 Hz
- ✅ USB2 / USB3 / USB-C
- ✅ NVMe storage
- ❔ Front panel audio: sounds is unbalanced and weird
- ❔ SD card reader: haven't tested
- ❌ Sleep/wake: Doesn't work
- ❌ Built in WLAN/Bluetooth: No but maybe [working soon](https://github.com/AppleIntelWifi/device-logs/issues/1)

## Hackintosh details

![](img/mac-os-screenshot.png)

config.plist: [EFI/CLOVER/config.plist](EFI/CLOVER/config.plist)

EFI directory: [EFI](EFI)

kexts:

- [USBInjectAll](https://bitbucket.org/RehabMan/os-x-usb-inject-all/downloads/): `0.7.1` (2018-11-09)
- [Lilu](https://github.com/acidanthera/Lilu): `1.4.5`
- [AppleALC](https://github.com/acidanthera/AppleALC): `1.5.0`
- [VirtualSMC](https://github.com/acidanthera/VirtualSMC): `1.1.4`
- [FakePCIID](https://bitbucket.org/RehabMan/os-x-fake-pci-id/downloads/): `1.3.15` (2018-10-27)
- [IntelMausi](https://github.com/acidanthera/IntelMausi): `1.0.3`

## Photos

[![](img/more-photos.png)](img)

## Hardware

### Specs

- Intel Core i5-8259U CPU (built in)
- Intel Iris Plus Graphics 655 (built in)
- 16GB RAM F4-2400C16D-16G
- XPG SPECTRIX S40G NVMe M.2 SSD
- TP-Link T3U AC1300 USB WLAN
- Alpine AM4 Passive CPU cooler, required some machining to fit
- Makerbeam open case structure
- Custom 3D printed CPU mounting brackets
- Custom 3D printed power switch bracket

### Power consumption and temperatures

Power measured at wall, temperature measured from built in sensors.

| State                                        | Power (watts) | CPU temp (°C) |
|----------------------------------------------|---------------|---------------|
| Powered off                                  | 0.9           | 0             |
| Booted OS, idle                              | 4-6           | 34            |
| Normal use with Chrome, AutoCAD, Spotify etc | 10-20         | 40-70         |
| Prime95 or stress                            | 44            | 94            |

### CAD files

[![](img/cad-header.png)](#)

Fusion 360 project file, Heatsink bracket STL and Switch bracket STL files are in: [cad-files](cad-files)
