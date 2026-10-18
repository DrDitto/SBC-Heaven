# 🌌 The SBC Heaven (Single Board Computer Resource Hub)

Welcome to **The SBC Heaven**, a centralized, community-driven repository designed to be the ultimate sanctuary for Single Board Computer (SBC) assets. Finding production-ready system images, Device Tree Blobs/Overlays (DTBs/DTBOs), and verified out-of-tree hardware drivers shouldn't be a struggle.

This repository hosts clean, tested, and optimized resources categorized logically by **SoC Family / Vendor** to streamline development, testing, and deployment.

---

## 📂 Repository Structure

The repository is organized by silicon vendor (e.g., `rockchip`, `allwinner`), with dedicated subdirectories for `drivers`, `dtb`, and compressed `images` structured by specific SoC sub-families (`rk356x`, `h61x`, etc.):

```text
.
├── allwinner
│   ├── drivers
│   ├── dtb
│   └── images
│       └── h61x
│           └── H61X_Debian13_minimal_kernel7.0_20260430.img
└── rockchip
    ├── drivers
    ├── dtb
    └── images
        └── rk356x
            ├── rk356x_minimal_k7.2.8.img.xz
            ├── rk356x_minimal_k7.3.0-rc5.img.xz
            └── rk356x_proxmox_9_2_20_k7.2.8.img.xz
## Technical Compliance Matrix

| Metric / Requirement | Rockchip (RK356x / RK3588) | Allwinner (H61x / A64) |
| :--- | :--- | :--- |
| **Mainline Linux Support (7.x+)** | ✅ Native | ✅ Native |
| **Open-Source Graphics Drivers** | ✅ Panfrost / Panthor | ✅ Lima |
| **Dynamic DTBO Overlay Support** | ✅ U-Boot / UEFI | ✅ U-Boot / UEFI |
| **Direct SPI Flash (`&sfc`) Control** | ✅ Supported | ✅ Supported |
| **`PREEMPT_RT` Determinism** | ✅ Validated | ✅ Validated |

---

## Conclusion

By strictly standardizing on **Rockchip** and **Allwinner**, the Meta Distribution enforces a lean, transparent Hardware Abstraction Layer (HAL). This design guarantees total architectural control from the low-level bootloader to the userspace runtime environment.
