# Bringing New Life to the Galaxy Tab A 10.1 (SM-T510)
## Goals

Dedicated to breathing life into the Samsung Galaxy Tab A 10.1 (SM-T510) through custom ROM development. Inspired by the great work of @Magendanz on the initial LineageOS 18.1 TWRP builds, lets pusg the boundaries of what's possible on this device.


## Moving Beyond GSIs

While projects like PHH and AndyYan GSIs revitalize older devices, they face challenges. Google's discontinued security support makes backporting patches difficult, and our device's aging Exynos ARM architecture adds another layer of complexity.


## The Challenges Ahead


**RAM Restrictions:** Modern Android versions ideally want 3GB+ of RAM, we are working with less than that.

**Outdated Kernel:** We're stuck with a legacy kernel (v4.4.xx), while newer Android requires features like eBPF which we have a semi-working implementation of



## Development Notes

I have left my development on the backburner as of late, medical studies take precedence over free time. Wish it was not the case.

- Starting my device tree from scratch, and aiming to carry out what I intended. 

### Changelog

- [gta3xlwifi-kernel](https://github.com/gta3xlwifi-dev/android_kernel_gta3xlwifi) - June 30, 2024: Import OEM changes and refactor kernel base on upstream Android common kernel (deprecated/4.4.p)
- [gta3xlwifi-device](https://github.com/gta3xlwifi-dev/android_device_samsung_gta3xlwifi) - July 1, 2024: Refactoring, messy codebase. Decided to start over for my own sanity, will likely do so with the AOSP tree

# How You Can Contribute


Testing: Download our experimental builds, provide feedback, and help us squash bugs 🐛!

Development: If you've got coding chops, dive into the codebase, suggest features, and work on optimizations.

Documentation: Help us create clear guides and tutorials to make the ROM accessible to everyone.

Spread the Word: Share our project with other Galaxy Tab A users and/or Developers.



# Getting Started

Prerequisites:
- [Odin v3.13.1](https://build.nethunter.com/samsung-tools/)
  - Be weary, plenty of ¨official¨ Odin links. Odin is Samsung´s proprietary software which has never been officially released by them
  - XDA threads or Nethunter repository, the most reputable sources for finding it. I choose the latter
- Fresh install or flash of the [latest available firmware](https://samfw.com/firmware/SM-T510/)
  - for us, this would be the T510XXU5CWA1 build.
 
ROM Downloads: 
- [Lineage-20](https://github.com/gta3xlwifi-dev/android_device_samsung_gta3xlwifi/releases/tag/20.0-20230901)
  - [XDA thread](https://xdaforums.com/t/rom-sm-t510-unofficial-lineageos-20-0-for-galaxy-tab-a-10-1-2019.4623077/)
 
- [Lineage-19.1](https://github.com/gta3xlwifi-dev/android_device_samsung_gta3xlwifi/releases/tag/19.1-20230403)
  - [XDA Thread](https://xdaforums.com/t/rom-sm-t510-unofficial-lineageos-19-1-for-galaxy-tab-a-10-1-2019.4494595/)
 

Installation Instructions: 
[XDA Thread](https://xdaforums.com/t/rom-sm-t510-unofficial-lineageos-20-0-for-galaxy-tab-a-10-1-2019.4623077/)
- I would refer to Magendanz official and initial post. The instructions are available above. For sake of availability, I will provide them down below.

# From OEM stock firmware:
- [Unlock bootloader](https://www.ifixit.com/Guide/How+to+unlock+the+bootloader+of+an+Android+Phone/152629)
- Power the device off
- Hold Vol Up & Vol Down buttons while plugging the USB-C from PC to tablet to enter Download mode
 
- Install custom ROM tarball (.tar.md5 file) to AP with Odin
- If TWRP launches, factory reset with Wipe->Format Data and reboot to system. (Not necessary for incremental upgrades.)

# From existing TWRP install:
- Hold Power & Vol Up during restart to enter TWRP recovery
- Tap Install, Install Image, select your update (.img file), OR Install via [ZIP archive](https://github.com/gta3xlwifi-dev/android_device_samsung_gta3xlwifi/releases/tag/20.0-20230901). 
- Factory reset with Wipe->Format Data. (Not necessary for incremental upgrades.)
- Reboot to system

Reporting Issues: 
- Ideally, right [here](https://github.com/gta3xlwifi-dev/.github/issues).

## Important Notice

These ROMs are under active development. Expect surprises (both good and bad!).  Please back up your data before flashing and always read instructions carefully.


Fun Fact: Did you know the Galaxy Tab A 10.1 was one of the first budget tablets with a full HD display? 
