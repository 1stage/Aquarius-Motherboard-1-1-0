# Aquarius Motherboard 1-1-0
Aquarius Motherboard 1-1-0 - Rev B
 
### by Sean P. Harrington
### sph@1stage.com
### http://aquarius.1stage.com
 
## Background
In general, the Aquarius hardware is fairly hardy. Few of the parts go bad, and the system just works, even when stored in harsh or unforgiving environments. Add to that the poor reception the computer had during its brief, 3-4 month sales window in 1983, and there is no REAL reason most people would be interested. But the Mattel Aquarius Computer was the first computer I ever owned. I learned first hand how to program in BASIC, and then how to hack together an audio cable to save those programs to my inexpensive Radio Shack cassette player. However I quickly grew out of it's limited functionality and moved on to a Commodore 64, and then an Apple Macintosh SE, and then Mac II, and then various Windows PCs. It wasn't until Summer of 2019 that I started getting back into retro computers, and it was the pang of guilt I felt in abandoning my first Aquarius that brought me back in.

## Purpose
The purpose of this project is to document and recreate the original Aquarius computer motherboard. This is a like-for-like replacement, and should fit in perfectly in place of the old motherboard. This baseline can be used by other enthusiasts (though we are few and far between) as a starting point for creating new modifications to the system, such as adding a composite video adapter (which I've done) to replace the stock RF modulator, or adding more modern components to "future proof" the system.

Additionally, there was a need to update and correct the "MEKO" schematic from 1986. It was drawn from the PAL board, and values for various components seemed to differ from what was commonly manufactured. From these new schematics, users are welcome to adapt and integrate their own ideas, OR to recreate the system in their eCAD program of choice.

## Caveats
* Some fixes were made:
  * The .1uF capacitor that was bodged under U6 has been given a proper set of pads beside U6.
  * Silkscreens were added, with all components being identified. Unfortunately, due to the poor quality of original Radofin documents on the Internet, I had to take a stance and perform a re-number of components, particularly resistors and capacitors. In some cases, these won't match original numbers, but every effort was made to get them as close as possible.
  * Both the PAL-only and NTSC-only components are marked, but only the components for the version being built should be used.
  * As much as possible, original trace paths were recreated (particularly CPU to expansion port), but the traces have been reduced to a 20 mil width on most signals, with all GND and power paths increased to 32 mil width.
  * GND pins now have thermal pads to make soldering and desoldering easier.
* The libraries within the Eagle folder are a mess. I apologize. The file "Aq 1-1-0b MB Libraries.png" in the docs folder shows a snapshot of what was in use at the point of publication of this project. It's a combination of the standard Eagle libraries, some copied/modified versions of those, and some of my own items. I'll eventually try to consolidate them into a single library file. Again, apologies.
* As of 10 AUG 2020, the Gerber files have NOT been used to create a PCB. That should be rectified by 01 SEP 2020, followed by at least TWO transplant/repopulation of stock components to fully confirm these PCB designs work.
* This design was taken from the NTSC version of the Aquarius Motherboard, Radofin part number 5931-4229 A. The values for all components are derived from the NTSC version, and where practical, PAL component values are noted on the schematic. As such, the "part number" embossed on these designs uses 5931-4229 AC to differentiate.
* The schematic does it's best to identify differences between the NTSC and PAL versions, usually with dashed lines surrounding the differences.

## Aquarius Hardware Development Roadmap
(A more up-to-date version of this list is at https://aquarius.1stage.com/hw-roadmap)

### Aquarius v1.0.0 : Baseline
* Aquarius v1.1.0 (Rev B): Aquarius 1 stock motherboard, like-for-like replacement, SANCTIONED FREE version. 
  * Aquarius v1.1.0.x : Users can fork at this level for their own purposes, UNSANCTIONED versions.
* Aquarius v1.2.0 : Aquarius 1 modernized motherboard, fits in Aquarius 1 case, unmodified port openings may be used differently, SANCTIONED PAID version.
  * Aquarius v1.2.1 : Integrated composite video ???
  * Aquarius v1.2.2 : Modern power supply ???
  * Aquarius v1.2.3 : Charmap, ROM, updates ???
* Aquarius v1.3.0 : Aquarius 1 motherboard, new layout, new case format, etc. ???
  * Aquarius v1.3.1 : New case design with mechanical keyboard, RGB output, proper serial, etc. ???

### Aquarius v2.0.0 : Baseline (FUTURE)
* Aquarius v2.1.0 : Aquarius 2 stock motherboard, like-for-like replacement, SANCTIONED FREE version.
  * Aquarius v2.1.0.x : Users can fork at this level for their own purposes, UNSANCTIONED versions.
  * Aquarius v2.1.1 : Aquarius 2 motherboard, updated with proper silk screen markings and ground planes, SANCTIONED PAID version.
  * Aquarius v2.1.2 : Aquarius 2 motherboard, updated with bodge fixes, modern component replacements, traces may be updated/optimized, SANCTIONED PAID version.
* Aquarius v2.2.0 : Aquarius 2 modernized motherboard, fits in Aquarius 2 case, unmodified port openings may be used differently, SANCTIONED PAID version.
  * Aquarius v2.2.1 : Charmap, ROM, etc updates ???
* Aquarius v2.3.0 : Aquarius 2 motherboard, new layout, new case format, etc. ???

### Aquarius v3.0.0 : Baseline (FUTURE)
New OPEN computer, modern, programmable system (new video system, RAM system, sound, etc.)
* Aquarius v3.1.0 : Aquarius 3 motherboard, SANCTIONED FREE version
