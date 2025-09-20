# ThinkMoth Expresscard to NVMe 
An ExpressCard to NVMe adapter, except this one actually ships! 

The ThinkMoth ExpressCard to NVMe is a low cost, open source adapter for using an M.2 2230/2242 NVMe SSD in an ExpressCard34/54 socket. It features a microSD card holder to let older machines boot from the SSD, and status LEDs for SD and PCIe activity so you can look at cool lights.  


Update 20/9/25:
Prototype PCBs have been ordered

![Front render](https://github.com/mothenjoyer69/thinkmoth-expresscard/blob/main/photos/front3d.png)
![Back render](https://github.com/mothenjoyer69/thinkmoth-expresscard/blob/main/photos/back3d.png)

# Features
- Bootable! Either with the native NVMe UEFI driver, or with a bootloader installed on the microSD card
- M.2 2242 *and* M.2 2230 support!
- Status LEDs for PCIe and uSD activity
- 3D printed case that I should probably start designing soon


# Booting from the SSD
Depending on how old your computer is, you will probably need a bootloader on a microSD card. Clover or Opencore work best and I will have working images you can use :)

# Questions?
1. What SSD works best?:
    - ExpressCard is super power limited with only 3v3@1A available to the SSD, so anything slower/low power drives should work fine. Higher end drives might have issues.
2. How fast is it?:
    - ExpressCard only gives you a PCIe 1x link, so depending on how old your laptop is, it should be anywhere from 250MB/s to 1GB/s (PCIe 1.0 to 3.0). Works out well with the limited power budget :3
3. Do all laptops work?:
    - Everything with an EC34/54 socket should work, including all generations of ThinkPads, Latitudes, Elitebooks etc. If you find something that doesn't, please let me know

# To-do
- Order intitial prototype PCBs [ ]
- List on tindie/lectronex [ ]
- Experiment with 1.5V -> 3.3V boost design [ ]

# Credits
A very big thank you to [Ambra](https://github.com/ambraglow/) for the original board outline, cutout, and EC footprint, and also to [Wifi](https://github.com/a-little-wifi/) and [Arya](https://github.com/CRImier/) and everyone else for all of the help and advice :3 

