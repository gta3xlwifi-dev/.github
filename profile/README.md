# Breathing Life into the Galaxy Tab A 10.1 (SM-T510)

**Goals**

This project is dedicated to revitalizing the Samsung Galaxy Tab A 10.1 (SM-T510) through custom ROM development. Building upon the excellent foundation laid by @Magendanz's initial LineageOS 18.1 TWRP builds, we aim to push the boundaries of what's possible on this device.

## Why Custom ROMs?

While projects like PHH and AndyYan GSIs breathe new life into older devices, they face limitations. Google's discontinued security support for this device makes backporting patches challenging, and its aging Exynos ARM architecture adds another layer of complexity. Custom ROMs offer a way to overcome these obstacles and provide a more up-to-date and optimized Android experience.

## Challenges We Face

* **RAM Restrictions:** Modern Android versions ideally require 3GB+ of RAM, but we're working with less.
* **Outdated Kernel:** We're limited by a legacy kernel (v4.4.xx), while newer Android versions need features like eBPF (which we have a semi-working implementation of).

## Development Status

**Note:** Development is currently on hold due to medical studies taking precedence. We hope to resume work soon!

* The device tree is being rebuilt from scratch for a cleaner foundation.
* AOSP tree refactoring is also planned.

### Changelog

* **gta3xlwifi-kernel:** June 30, 2024: Imported OEM changes and refactored the kernel base on upstream Android common kernel (deprecated/4.4.p).
* **gta3xlwifi-device:** July 1, 2024: Refactored the messy codebase. Decided to start over for better maintainability. Will likely do the same with the AOSP tree.

## How You Can Contribute

* **Testing:** Download our experimental builds, provide feedback, and help us identify and fix bugs.
* **Development:** If you have coding skills, dive into the codebase, suggest features, and work on optimizations.
* **Documentation:** Help us create clear guides and tutorials to make the ROM accessible to everyone.
* **Spread the Word:** Share our project with other Galaxy Tab A users and developers.

## Getting Started

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

**Reporting Issues:**

Please report any issues [here](https://github.com/gta3xlwifi-dev/.github/issues).

## Important Notice

These ROMs are under active development. Expect things to change and potential bugs. **Back up your data before flashing** and always read instructions carefully.

**Fun Fact:** The Galaxy Tab A 10.1 was one of the first budget tablets to feature a full HD display!
