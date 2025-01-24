# Breathing Life into the Galaxy Tab A 10.1 (SM-T510)

**Goals**

This project aims to give life to the Samsung Galaxy Tab A 10.1 (SM-T510) through custom ROM development, by building upon the foundation laid by @Magendanz's initial LineageOS 18.1 TWRP builds.

While projects like PHH and AndyYan GSIs give new life into older devices, they face limitations. Google's discontinued security support for this device makes backporting patches challenging, and the aging Exynos ARM architecture adds another layer of trouble

## Challenges We Face

* **RAM Restrictions:** Modern Android ideally needs 3GB+ of RAM, we're working with less than that
* **Outdated Kernel:** We're limited by a legacy kernel (v4.4.xx), while newer Android versions need features like eBPF

## Development Status

**Note:** Development is on hold due to my medical studies taking precedence

**Prerequisites:**

* **Odin v3.13.1:**
    * Be cautious of "official" Odin links. Odin is Samsung's proprietary software and has never been officially released.
    * Reputable sources: XDA threads or the Nethunter repository. 
* Fresh install or flash of the [latest available firmware](https://samfw.com/firmware/SM-T510/) (T510XXU5CWA1).

**ROM Downloads:**

* **Lineage-20:** 
    * XDA Thread: [Link](https://xdaforums.com/t/rom-sm-t510-unofficial-lineageos-20-0-for-galaxy-tab-a-10-1-2019.4623077/)
* **Lineage-19.1:**
    * XDA Thread: [Link](https://xdaforums.com/t/rom-sm-t510-unofficial-lineageos-19-1-for-galaxy-tab-a-10-1-2019.4494595/)

**Installation Instructions:**

Refer to the [XDA Thread](https://xdaforums.com/t/rom-sm-t510-unofficial-lineageos-20-0-for-galaxy-tab-a-10-1-2019.4623077/) for detailed instructions.

**Brief Summary:**

* **From OEM Stock Firmware:**
    1. Unlock the bootloader.
    2. Enter Download mode (Vol Up + Vol Down while plugging in USB-C).
    3. Use Odin to flash the custom ROM (.tar.md5 file) to AP.
    4. If TWRP launches, factory reset and reboot to system.
* **From Existing TWRP Install:**
    1. Enter TWRP recovery (Power + Vol Up during restart).
    2. Install the update (.img file or ZIP archive).
    3. Factory reset (if not an incremental upgrade).
    4. Reboot to system.

## Notice

These ROMs are under active development. Expect things to change and potential bugs. **Back up your data before flashing** and always read instructions carefully.

**Fun Fact:** The Galaxy Tab A 10.1 was one of the first budget tablets to feature a full HD display!
