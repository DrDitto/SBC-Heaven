# 🌌 SBC Heaven (Single Board Computer Resource Repository)

Welcome to **SBC Heaven**—the ultimate sanctuary for Single Board Computer enthusiasts, developers, and embedded Linux tinkerers. 

The primary vision of this repository is to serve as a comprehensive, well-structured, and reliable hub where you can find **everything you need for your SBCs in one single place**. No more hunting down broken links or hunting through obscure forums; here, everything is organized neatly by **SoC Family and Chipset**.

---

## 🚀 What You Will Find Here

Everything in this repository is categorized by **SoC / Chip Family** (e.g., `rk356x`, `rk3588`, `px30`, etc.) to ensure seamless navigation:

* 📀 **Ready-to-Use OS Images**: Pre-built, shrinked, and optimized images (Minimal, Proxmox, bleeding-edge kernels like `7.3.0-rc5`, etc.) ready to flash.
* 🌳 **Device Tree Blobs & Overlays (.dtb / .dtbo)**: Cleaned and tested Device Tree sources and compiled overlays (e.g., NPU overlays, custom pinouts).
* ⚙️ **Drivers & DKMS Modules**: Pre-compiled kernel modules, out-of-tree drivers, and hardware acceleration libraries (e.g., RKNN RT, Mali GPU drivers).
* 🔧 **Kernel Configurations & Patches**: Tested `.config` files and custom patchsets for edge and bleeding-edge kernel trees.

---

## 📁 Repository Structure

```text
.
├── rk356x/
│   ├── images/       # Flashing-ready OS images (.img / .img.xz)
│   ├── dtb/          # Device Tree Blobs and Overlays (.dtbo)
│   └── drivers/      # DKMS modules and runtime drivers (e.g., RKNN)
├── rk3588/
│   ├── images/
│   ├── dtb/
│   └── drivers/
└── README.md
```

---

## 🌟 Key Features

* **Shrinked & Optimized:** Images are processed with `pishrink` to guarantee fast downloads and automated partition expansion on first boot.
* **Bleeding-Edge Kernel Support:** Track and deploy custom build setups featuring up-to-date Linux kernels.
* **Hardware Acceleration First:** Ready-to-use configurations for hardware NPUs, GPUs, and specialized hardware interfaces.

---

## 🤝 Contributing

Contributions are welcome! If you have optimized images, working DTB overlays, or driver patches for any SoC family, feel free to open a Pull Request.

---
*Maintained with passion for low-level board bring-up and embedded system tweaking.*
