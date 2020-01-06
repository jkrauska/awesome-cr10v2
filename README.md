# awesome-cr10v2
Notes and info about Creality CR-10 V2 3D Printers


## Before You Buy

## Other Printers I Considerd
- [Tevo Tornado](https://tevo3dprinterstore.com/) - well loved CR-10 clone with some nice features
- [Creality Ender-5 Pro](https://www.creality3d.shop/collections/ender-series-3d-printer/products/creality3d-ender-5-pro-3d-printer) - smaller build volume, nice upgrades, not sure about whole-plate Z motion
- [LulzBot Mini2](https://www.lulzbot.com/store/printers/lulzbot-mini-2)  - much more $$$ - less hassle?


### Other CR-10 Variants

Wow it's confusing to navigate the CR-10 product line. Here's the best I could figure out

- CR-10 (original - orange) 300x300x400mm
- CR-10 v2 (reinforced frame, upgraded components)
- CR-10S (first CR-10 Upgrade, filament sensor and dual Z)
- CR-10S Pro (electronics in stand, touchscreen UI, auto bed leveling)
- CR-10 S4,Max,S5 (bigger prints, other upgrades) 400x400x400mm, 450x450x470, 500500x500mm
- CR-10 Mini (smaller than CR-10, bigger than Ender 3) 300x220x300mm
- CR-X (dual extruders)

### Why CR-10v2
- Dual Z screws
- Better PSU
- Quieter Drivers
- Better Head Cooling
- Metal Extruder
- Easy to add BLTouch

### Resellers

Websites for Creality:
 - https://www.creality.com/
 - https://www.creality3dofficial.com/
 - https://creality3d.shop/  


## Getting started

### Shipping

My box was pretty banged up, but nothing inside looked too worse for wear.

### Build
There are LOTs of build videos online where people will live build the printer and you can follow along.

Quick Gotachas:
 - There should be an insert that gives details about the end caps in the front for the arm attachment and installing the z-axis limiter switch. (which I later removed with the BLTouch)
 - Be sure to flip voltage switch from 230V to 115V
 - Check for loose bolts or other wobbly things that might need tightening.

### Firmware

My CR-10V2 shipped with firmware CR-10V2 1.1.6 V, which matched what was on their [website](https://www.creality.com/download/firmware_c0008).

I later needed to install the newer firmware with BLTouch V2 support (1.1.6 2019-11-13), and I was able to find it [here](https://www.creality3dofficial.com/pages/firmware-download).  

I have a Mac, so I wasn't able to use Creality's slicer software, but I WAS able to upgrade the firmware using Cura.


### Software

I downloaded [Utlimaker Cura](https://ultimaker.com/software/ultimaker-cura) as a slicer for OSX.

I also want to install [Octoprint](https://octoprint.org/) on a RaspberryPi to attach a camera to check on builds.  

There's an AI powered build failure detector called [The Spaghetti Detective](https://plugins.octoprint.org/plugins/thespaghettidetective/) which looks awesome.

I downloaded [FreeCAD](https://www.freecadweb.org/) to edit models, but haven't tried it yet.



## Troubleshooting

### Bed wobble
After building, my printing surface/bed was very wobbly   You can remove the glass and heating surface and then tighten up the bolts on the glides that run along the Y-Axis to remove the wobble. 

## Enhancements

### BLTouchV2
I got the [BLTouchV2 kit](https://www.amazon.com/Creality-3D-Printer-Leveling-Sensor/dp/B07Z5P9P1S) for ~$60 -- it's specifically made for the CR-10 V2 and didn't have to made any modifications to the wiring blocks and the mount 'just worked'.

I'm still not sure I fully understand bed leveling and how it's related to Z-offset, but you can watch as it measures the depth in 9 locations on the grid.  It measures in each location twice.  Once faster and once slower.  I've made adjustments to the thumb wheels to make all of those measurements be less than 0.3mm off. 

I set the Z offset per the instructions, but I don't know if that then adjusts ALL of my Z position settings.


## Resources

### Models
- [Yeggi Model Search](https://www.yeggi.com/)

- [Thingiverse](https://www.thingiverse.com/)
- [Cults3D](https://cults3d.com/) - Nice StarWars collections



### Web
- [Facebook Group](https://www.facebook.com/groups/CrealityCR10/) - Very active
- [Reddit Groupd for CR-10](https://www.reddit.com/r/CR10)
- [Creality Experts](https://www.crealityexperts.com/gettingstarted)
- [Thingiverse CR-10 Forum](https://www.thingiverse.com/groups/creality-cr-10)


### Video Content
- [Filament Friday](https://www.youtube.com/user/beginnerelectronics/videos)


## Hacks I Want To Checkout

- USB Power Block so Octoprint doesn't power LCD. 
- Is it safe to setup Cura to heat bed and nozzle at the same time (wattage draw ok for PSU?)
- Capricorn Bowden Tubing is better?
- Geared Idler Pullys
- Is PLA strong enough for GearWall hook?
- Why bigger nozzles?
- Tweaking temps? Volumes??
- Clean hotend? Lots of reports of metal coils stuck in hotend?
- Spacer to push spring on extruder?
- Bed temp 70?  not 60 (default or 45?)
- Hairspray to help with attach?
