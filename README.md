# Infinity-X-3.9-QPR2-for-Realme-8i-Narzo-50-spaced

## 🛠️ System & Performance
* **Resource Optimization:** Reworked `PowerHint` with policy-based nodes and tuned `schedutil` for more responsive CPU frequency scaling.
* **Memory Management:** Boosted **zRAM to 70%** of total RAM with **70 swappiness**, disabled writeback, and updated LMK for improved multitasking.
* **Graphics & Rendering:** Enhanced smoothness by moving to **4 buffers** in SurfaceFlinger, increasing sampling frequency, and adopting Motorola phase offsets.
* **GPU Boost:** Patched **MediaTek GED** permissions to allow `gpu_boost_level 100` during high-load tasks, ensuring zero dropped frames.
* **Cleanup:** Purged legacy MediaTek gauge, power properties, tracing tools, and compat namespaces.

## 📺 Display & UI
* **Animations:** Switched to **linear interpolators** for consistent motion and simplified transitions.
* **Jank Reduction:** Optimized the link between SurfaceFlinger and the MTK display driver to eliminate micro-stutters during heavy UI transitions.
* **UI Refinement:** Added **rounded corner support**, reduced blur radius, and adjusted status bar padding.

## 🔊 Connectivity & Audio
* **NFC:** Upgraded to the modern **AIDL NXP NFC HAL** stack.
* **Audio Overhaul:** Integrated **Dolby Sony** audio for a premium sound experience.
* **Streamlining:** Stripped unused codecs, disabled PCM dumping, and removed MTK encoder performance hints.

## 🛡️ Security, Stability & OTA
* **Certification:** ROM is now **fully signed** and passes all **3 Play Integrity checks** (Device Certified).
* **Updates:** Integrated **OTA Update** support for seamless future releases.
* **Security & SEPolicy:** Disabled Factory Reset Protection (FRP) and authored custom vendor rules to resolve **sysfs_ged** permission denials.
* **Thermal Tuning:** Adjusted thresholds to prevent aggressive throttling during sustained high-performance encoding.

## ⚙️ Core & Runtime
* **ART/Dalvik:** Reverted dynamic heap overrides and streamlined property initializations.
* **Legacy Removal:** Cleaned up Android 11 `libinit` adaptations and stale system includes.
* **Compatibility:** Updated `system/core/base` logic and patched blobs for `libtinyxml2-v34` compatibility.

## 🏗️ Build System & Fixes
* **Standardization:** Converted `rootdir` to **Blueprint**, renamed Lineage overlays, and removed duplicate configs.
* **Bug Fixes:** Corrected permission errors for `opluserserve1` and resolved "Permission Denied" issues for kernel performance nodes.

## 🚀 HUGE THANKS TO @HELLINFIX FOR THE TREES AND ALL THE HELP 🫡
## 🤝 Thanks to @crss5G for teaching me how to implement OTA updates
## 🎵 Thanks to @ViaanLarryROMS for the assistance in adding Sony Dolby
