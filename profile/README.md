# Android Development for POCO X7 Pro (rodin)

Device configuration for POCO X7 Pro 5G / Redmi Turbo 4

The POCO X7 Pro / Redmi Turbo 4 (codenamed "rodin") is an upper mid-range smartphone from Xiaomi, announced and released on January 09, 2025. This organization hosts device trees, kernel sources, and hardware layers for Android development on rodin, focusing on clean bring-up, stability, and performance.

### Its purpose is intended for personal individual use for now
 
## Device picture
![POCO X7 Pro](https://github.com/Digimend-X-Rodin/.github/blob/main/profile/1a097d170ec6940798552eee961fc641.webp)

## Device specifications

| Basic            | Spec Sheet                                                                                      |
|------------------|-------------------------------------------------------------------------------------------------|
| SoC              | Mediatek Dimensity 8400 Ultra (MT6899)                                                          |
| CPU              | Octa-core (1x3.25 GHz Cortex-A725 & 3x3.0 GHz Cortex-A725 & 4x2.1 GHz Cortex-A725)              |
| GPU              | Mali-G720 MC7                                                                                   |
| Memory           | 8/12GB, LPDDR5X                                                                                 |
| Storage          | 256/512GB, UFS 4.0                                                                              |
| Shipped Android  | Android 15, HyperOS 2                                                                            |
| Battery          | Non-removable Li-Ion 6550/6000 mAh                                                              |
| Dimensions       | 160.8 x 75.2 x 8.3 mm (6.33 x 2.96 x 0.33 in)                                                   |
| Weight           | 195 g or 198 g (6.88 oz)                                                                        |
| Display Type     | AMOLED, 68B colors, 120Hz, 1920Hz PWM, Dolby Vision, HDR10+, 1400 nits (HBM), 3200 nits (peak)  |
| Display Size     | 6.67 inches (~88.8% screen-to-body ratio)                                                       |
| Resolution       | 1220 x 2712 pixels, 20:9 ratio (~446 ppi)                                                       |
| Rear Camera 1    | 50 MP, f/1.5, 26mm (wide), 1/1.95", 0.8µm, PDAF, OIS                                           |
| Rear Camera 2    | 8 MP, f/2.2, 15mm (ultrawide), 1/4.0", 1.12µm                                                   |
| Front Camera     | 20 MP, f/2.2, 25mm (wide), 1/4.0", 0.7µm                                                        |

## Maintainer

- Omkar Parte (RAM-UNLOK) — novice developer  
  GitHub: https://github.com/RAM-UNLOK

## Credits For Base DT and Much More.....

- Major Thanks To [rthedream](https://t.me/rthedream) [rthedream](https://github.com/xyzuniverse)  
  GitHub: https://github.com/mt6899-rodin

## Repositories

- Device tree: https://github.com/Digimend-X-Rodin/android_device_xiaomi_rodin
- Mediatek sepolicy_vndr: https://github.com/Digimend-X-Rodin/android_device_mediatek_sepolicy_vndr  
- Mediatek hardware: https://github.com/Digimend-X-Rodin/android_hardware_mediatek  
- Xiaomi hardware: https://github.com/Digimend-X-Rodin/android_hardware_xiaomi  
- Kernel: https://github.com/Digimend-X-Rodin/android_device_xiaomi_rodin-kernel

## Sync and clone

Run each command separately (each block is one-click copy):


### Common Command For Source Sync

```
repo init -u https://github.com/Lunaris-AOSP/android -b 16 --git-lfs --depth=1
```

```
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```

### Commands For DT Clone

```
git clone https://github.com/Digimend-X-Rodin/android_device_xiaomi_rodin.git device/xiaomi/rodin
```

```
git clone https://github.com/Digimend-X-Rodin/android_device_mediatek_sepolicy_vndr.git -b lineage-23.2 device/mediatek/sepolicy_vndr
```

```
git clone https://github.com/Digimend-X-Rodin/android_hardware_mediatek.git -b lineage-23.2 hardware/mediatek
```

```
git clone https://github.com/Digimend-X-Rodin/android_hardware_xiaomi.git -b lineage-23.0 hardware/xiaomi
```

```
git clone https://github.com/Digimend-X-Rodin/android_device_xiaomi_rodin-kernel.git -b TheCloverProject device/xiaomi/rodin-kernel
```

```
git clone --depth=1 https://gitlab.com/ram-unlok/vendor_xiaomi_rodin.git -b TheCloverProject vendor/xiaomi/rodin
```

```
git clone https://github.com/mt6899-rodin/android_vendor_mediatek_ims.git vendor/mediatek/ims
```

Optional If Souce Doesnt Have It
```
git clone https://github.com/ProjectInfinity-X/vendor_infinity-priv_keys-template.git vendor/infinity-priv/keys
```

```
git clone --depth=1 git://git.kernel.org/pub/scm/linux/kernel/git/stable/linux.git -b linux-6.6.y kernel/xiaomi/rodin
```

```
git clone https://github.com/swiitch-OFF-Lab/packages_apps_DolbyUI.git -b 16.0 packages/apps/DolbyUI
```

```
git clone https://github.com/swiitch-OFF-Lab/hardware_dolby.git -b moto-1.4 hardware/dolby
```

```
git clone --depth=1 https://github.com/TogoFire/packages_apps_ViPER4AndroidFX.git packages/apps/ViPER4AndroidFX
```

```
git clone --depth=1 https://gitlab.com/ram-unlok/bcr.git vendor/bcr
```

```
git clone --depth=1 https://gitlab.com/ram-unlok/vendor_PixelPlay.git vendor/PixelPlay
```

```
git clone https://rakmoparte@bitbucket.org/ram-unlok/vendor_gcam.git vendor/gcam
```

```
./extract-files.py Path/To/Dumpyara/Extract
```

## Notes

- Place these trees in the Android source under the listed paths (device/xiaomi/rodin, hardware/mediatek, hardware/xiaomi, etc.).  
- Execute the commands from the source root so relative destinations resolve correctly.  
- Build steps vary by ROM; check the ROM’s docs for the correct lunch combo and targets.
