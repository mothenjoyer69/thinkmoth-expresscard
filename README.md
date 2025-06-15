# ThinkMoth Expresscard to NVMe
An ExpressCard to NVMe adapter, except this one actually ships! Its also entirely open source from the start, and features both M.2 2242 *and* M.2 2230 support, as well as an SD card slot to let you boot from the SSD on older systems

It's still a work in progress, but I'm hoping to get it produced and tested soon!

![Front render](https://github.com/mothenjoyer69/thinkmoth-expresscard/blob/main/photos/front3d.png)
![Back render](https://github.com/mothenjoyer69/thinkmoth-expresscard/blob/main/photos/back3d.png)

# Features
- Bootable! Either with the native NVMe UEFI driver, or with a bootloader installed on the microSD card
- M.2 2242 *and* M.2 2230 support. On the same board. :3
- Status LEDs for PCIe and microSD activity
- 3D printed case that I should probably start designing soon

# Booting from the SSD
Depending on how old your laptop/device is, you will either be able to boot natively without an issue, or you will need a bootloader on the microSD card. I've picked Opencore for this, and will add more info here later :)

Whenever I get around to it, images will be available in this repo but for now you just to have to close your eyes and imagine.

# Questions?
1. What SSD works best?:
    - ExpressCard is super power limited with only 3v3@1A available to the SSD, so avoid higher end drives. WD Blues etc should be a safe bet, but I'll list any and all tested drives here too.
2. How fast is it??
    - ExpressCard only gives you a PCIe 1x link, so depending on how old your laptop is, it should be anywhere from 250MB/s to 1GB/s (PCIe 1.0 to 3.0)
3. Is the SD card really necessary?
    - It runs the bootloader for anything old enough to not ship NVMe drivers in firmware. If you are running a newer device, or Coreboot, you don't need the SD.

# To-do
- Sanity check layout and placement of SD card reader [ ]
- Verify PCIe routing [ ]
- Sanity check ExpressCard design requirements [ ]
- Experiment with 1.5V -> 3.3V boost design [ ]
- Prototype PCB run :3 [ ]

# Credits
A very big thank you to [Ambra](https://github.com/ambraglow/) for the original board outline, cutout, and EC footprint!

Thanks to everyone at Hackmods for all of the help and advice provided :3 
