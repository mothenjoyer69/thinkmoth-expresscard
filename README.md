# ThinkMoth Expresscard to NVMe 
An ExpressCard to NVMe adapter, except this one actually ships! Its also entirely open source from the start, and features both M.2 2242 *and* M.2 2230 support, as well as an SD card slot to let you boot from the SSD on older systems. 

WIP for now :3

![Front render](https://github.com/mothenjoyer69/thinkmoth-expresscard/blob/main/photos/front3d.png)
![Back render](https://github.com/mothenjoyer69/thinkmoth-expresscard/blob/main/photos/back3d.png)

# Features
- Bootable! Either with the native NVMe UEFI driver, or with a bootloader installed on the microSD card
- M.2 2242 *and* M.2 2230 support. On the same board. :3
- Status LEDs for PCIe and microSD activity
- 3D printed case that I should probably start designing soon

# Booting from the SSD
Depending on how old your computer is, you will probably need a bootloader on a microSD card. Clover or Opencore work best and I will have working images you can use :)

# Questions?
1. What SSD works best?:
    - ExpressCard is super power limited with only 3v3@1A available to the SSD, so anything rated *around* that should be okay.
2. How fast is it?:
    - ExpressCard only gives you a PCIe 1x link, so depending on how old your laptop is, it should be anywhere from 250MB/s to 1GB/s (PCIe 1.0 to 3.0). Works out well with the limited power budget :3

# To-do
- Sanity check layout and placement of SD card reader [*]
- Verify PCIe routing [*]
- Sanity check ExpressCard design requirements [*]
- Experiment with 1.5V -> 3.3V boost design [ ]
- Prototype PCB run :3 [in progress]

# Credits
A very big thank you to [Ambra](https://github.com/ambraglow/) for the original board outline, cutout, and EC footprint, and also to [Wifi](https://github.com/a-little-wifi/) and [Arya](https://github.com/CRImier/) and everyone else for all of the help and advice :3 
