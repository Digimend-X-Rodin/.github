
<h1 align="center">📱 Android Development for POCO X7 Pro (rodin)</h1>

<p align="center">
  <strong>Device configuration for POCO X7 Pro 5G / Redmi Turbo 4</strong><br>
  <i>An upper mid-range smartphone from Xiaomi, released on January 09, 2025.</i>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Android-16-3DDC84?style=for-the-badge&logo=android&logoColor=white" alt="Android 16" />
  <img src="https://img.shields.io/badge/SoC-Dimensity_8400_Ultra-blue?style=for-the-badge" alt="Dimensity 8400 Ultra" />
  <img src="https://img.shields.io/badge/Status-Active-success?style=for-the-badge" alt="Status Active" />
</p>

> [!NOTE]
> This organization hosts device trees, kernel sources, and hardware layers for Android development on `rodin`, focusing on clean bring-up, stability, and performance.
> Its purpose is intended for **personal use** and **public releases**.

<p align="center">
  <img src="https://github.com/Digimend-X-Rodin/.github/blob/main/profile/1a097d170ec6940798552eee961fc641.webp" 
       alt="POCO X7 Pro" 
       style="padding: 0 50px;">
</p>

---

## 📊 Device Specifications

| Component | Specification |
| :--- | :--- |
| 📱 **SoC** | Mediatek Dimensity 8400 Ultra (MT6899) |
| 🧠 **CPU** | Octa-core (1x3.25 GHz Cortex-A725 & 3x3.0 GHz Cortex-A725 & 4x2.1 GHz Cortex-A725) |
| 🎮 **GPU** | Mali-G720 MC7 |
| 💾 **Memory** | 8/12GB, LPDDR5X |
| 💽 **Storage** | 256/512GB, UFS 4.0 |
| 🤖 **Shipped OS**| Android 15, HyperOS 2 |
| 🔋 **Battery** | Non-removable Li-Ion 6550/6000 mAh |
| 📏 **Dimensions**| 160.8 x 75.2 x 8.3 mm (6.33 x 2.96 x 0.33 in) |
| ⚖️ **Weight** | 195 g or 198 g (6.88 oz) |
| 📺 **Display** | AMOLED, 68B colors, 120Hz, 1920Hz PWM, Dolby Vision, HDR10+, 1400 nits (HBM), 3200 nits (peak) |
| 📐 **Size & Res**| 6.67 inches (~88.8% screen-to-body), 1220 x 2712 pixels, 20:9 ratio (~446 ppi) |
| 📸 **Rear Cam** | 50 MP, f/1.5, 26mm (wide), OIS **+** 8 MP, f/2.2, 15mm (ultrawide) |
| 🤳 **Front Cam** | 20 MP, f/2.2, 25mm (wide) |

---

## 👤 Maintainer & Credits

**Maintainer:** Omkar Parte (RAM-UNLOK) — *novice developer*

   🔗 **GitHub:** [@RAM-UNLOK](https://github.com/RAM-UNLOK)

**Special Thanks For Base DT & References:**
*   🥇 [@rthedream](https://github.com/xiaomi-mt6899-dev) for base trees
*   🤝 [Duchamp Development](https://github.com/mt6897-devs) for reference
*   🤝[Nothing-2A](https://github.com/Nothing-2A) for reference

**Major Thanks To All Our Group Testers ❤️**

---

## 📁 Repositories

| Component | Repository Link |
| :--- | :--- |
| 🌳 **Device Tree** | [android_device_xiaomi_rodin](https://github.com/Digimend-X-Rodin/android_device_xiaomi_rodin) |
| 🛡️ **Sepolicy VNDR** |[android_device_mediatek_sepolicy_vndr](https://github.com/Digimend-X-Rodin/android_device_mediatek_sepolicy_vndr) |
| ⚙️ **MTK Hardware** | [android_hardware_mediatek](https://github.com/Digimend-X-Rodin/android_hardware_mediatek) |
| ⚙️ **Xiaomi Hardware**|[android_hardware_xiaomi](https://github.com/Digimend-X-Rodin/android_hardware_xiaomi) |
| 🐧 **Kernel Source** | [android_device_xiaomi_rodin-kernel](https://github.com/Digimend-X-Rodin/android_device_xiaomi_rodin-kernel) |

---

## 🛠️ Sync and Clone

> [!TIP]
> **One-Click Copy:** click the **copy icon** in the right corner. Run each command separately from your source root.

### 🔄 Source Sync

*(Common command for source sync. Uses `--depth=1` to save storage space).*
```
--depth=1
```
```
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```

### 📥 DT Clone Commands

*Click to copy and run individually:*

```
git clone https://github.com/Digimend-X-Rodin/android_device_xiaomi_rodin.git device/xiaomi/rodin
```
```
git clone https://github.com/Digimend-X-Rodin/android_device_mediatek_sepolicy_vndr.git device/mediatek/sepolicy_vndr
```
```
git clone https://github.com/Digimend-X-Rodin/android_hardware_mediatek.git hardware/mediatek
```
```
git clone https://github.com/Digimend-X-Rodin/android_hardware_xiaomi.git hardware/xiaomi
```
```
git clone https://github.com/Digimend-X-Rodin/android_device_xiaomi_rodin-kernel.git device/xiaomi/rodin-kernel
```
```
git clone --depth=1 https://gitlab.com/ram-unlok/vendor_xiaomi_rodin.git vendor/xiaomi/rodin
```

<details>
<summary><b> ➕ Optional Commands (Click to expand) </b></summary>
<br>

*Clone this if your ROM source doesn't already include signing keys:*
```
git clone https://github.com/ProjectInfinity-X/vendor_infinity-priv_keys-template.git vendor/infinity-priv/keys
```

```
git clone https://github.com/swiitch-OFF-Lab/packages_apps_DolbyUI.git -b 16.0 packages/apps/DolbyUI
```
```
git clone https://github.com/swiitch-OFF-Lab/hardware_dolby.git -b sony-1.5 hardware/dolby
```
```
git clone https://gitlab.com/ram-unlok/bcr.git vendor/bcr
```
```
git clone https://gitlab.com/ram-unlok/vendor_PixelPlay.git vendor/PixelPlay
```
```
git clone --depth=1 git://git.kernel.org/pub/scm/linux/kernel/git/stable/linux.git -b linux-6.6.y kernel/xiaomi/rodin
```
```
git clone https://github.com/TogoFire/packages_apps_ViPER4AndroidFX.git packages/apps/ViPER4AndroidFX
```
```
git clone https://rakmoparte@bitbucket.org/ram-unlok/vendor_gcam.git vendor/gcam
```
</details>

<br>

### 📦 Extract Vendor Files

```
./extract-files.py Path/To/Dumpyara/Extract
```

---
## 📝 Notes

> [!IMPORTANT]
> *   **Directory:** Place these trees in the Android source under the strictly listed paths (`device/xiaomi/rodin`, `hardware/mediatek`, etc.).
> *   **Context:** Execute the commands from the **source root** so relative destinations resolve correctly.
> *   **Building:** Build steps vary by ROM; check the specific ROM’s documentation for the correct `lunch` combo and build targets.
