**Since APatch APP already supports in-APP upgrades, this project has lost its meaning. Perhaps the biggest benefit is custom KernelPatch patching, but this feature is very stable and requires no maintenance.**

**Well, then it's time to say goodbye.**

## **EOL**

---

# APatch Auto Patch Tool

A script that provides custom patching options.

[中文](./README_CN.md)

---

This script has the following functions:

- User-specified image path or get from current Android device.  
- User-specified KernelPatch version. Or default, latest release.  
- User-specified SuperKey.[What is SuperKey?](https://github.com/bmax121/APatch/blob/main/docs/en/faq.md#what-is-superkey)  
- Only patch but not install support.

---

## Usage

- Open Termux

- Prepare

```bash
cd ${HOME}
curl -LO https://raw.githubusercontent.com/nya-main/APatchAutoPatchTool/main/AAP.sh
chmod +x AAP.sh
```

*After this, You can directly run AAP.sh after command tsu is executed.*

- Run

Usage:
```
APatch Auto Patch Tool
Written by nya
Version: 1.0.0
Current DIR: /home/nya/APatchAutoPatchTool

-h, -v,                 print the usage and version.

-i [BOOT IMAGE PATH],   specify a boot image path.
-n,                     do not install the patched boot image, save the image in /storage/emulated/0/patched_boot.img, or on Linux /home/nya/patched_boot.img.
-k [RELEASE NAME],      specify a kernelpatch version [RELEASE NAME].
-s "STRING",            specify a superkey. Use STRING as superkey.
-S,                     Install to another slot (for OTA).
-V,                     verbose mode.
```

---

## TODO

- [x] User-specified boot image path.  
- [x] User-specified Superkey.  
- [x] User-specified KernelPatch version.  
- [x] Other terminal software support(e.g. MT).  
- [x] Linux Support.  

---


If you encounter any issues, please submit a issue on github or provide feedback to me: [Telegram](https://t.me/RhineNya)

---

Credits:

- [Magisk](https://github.com/topjohnwu/magisk): For magiskboot

- [KernelPatch](https://github.com/bmax121/KernelPatch): For kptools and kpimg
