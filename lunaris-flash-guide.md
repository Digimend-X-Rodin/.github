🛠 Installation Guide

❗️ Pre-requisites:
- Firmware: If you are coming from Modded Stock or HOS2, it is highly recommended to flash the latest HOS3 Global first before installing this ROM.
- Clean Flash is RECOMMENDED

Step 1: Flash Boot Images ( Mandatory )
Connect your device in Fastboot mode and run:
```bash
fastboot flash vendor_boot vendor_boot.img
```
```bash
fastboot flash boot boot.img
```
```bash
fastboot reboot recovery
```
Step 2: Format & Sideload
1. Factory Reset: Go to Factory Reset -> Format Data/Factory Reset. ( skip for dirty flashing )
2. Prepare Sideload: Go to Apply Update -> Apply from ADB.
3. Sideload ROM: From your computer using:
```bash
adb sideload filename.zip
```
4. Finally: You will asked : "Reboot to recovery?" -> Select YES.

Step 3:  Sideload Gapps ( Skip if not vanilla build )
1. Finish: Once back in recovery, flash gapps now else
```bash
adb sideload gapps.zip
```
2. Reboot System Now.

💡 Pro-Tips:
- If your fod sensors or speaker feel uncalibrated after the first boot, go to Settings > Xiaomi Parts to calibrate them.
- The first Day You May Feel Heating, Battery Drain and Laggy. Please be patient!