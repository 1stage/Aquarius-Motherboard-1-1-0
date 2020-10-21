# Errata - Rev B Boards
Updated 21 OCT 2020, by Sean Harrington<br/>

## Abstract
Erratas to Rev B board. Corrections are made in Rev C.

## New
* Pin 15 on U6 needs to be GND (currently open)

## Feedback Needed
* None

## Resolved
* R14 = 680R (not 2.2K) - Compromised. R14 will show 2.2k for NTSC and 680 for PAL. 19 OCT, SPH in SCHEMATIC and BOARD 1-1-1c files.
* R15 = 2.2K (not 1.2k) - Compromised. R15 will show 1.2k for NTSC and 2.2k for PAL. 19 OCT, SPH in SCHEMATIC and BOARD 1-1-1c files.
* Pin 1 label on U13 against wrong pin (Pin 14) - Resolved 19 OCT, SPH in SCHEMATIC and BOARD 1-1-1c files.
* C1 = 10uf - Compromised. C1 will show 1uF @ 16v for NTSC and 10uF @ 50v for PAL. 19 OCT, SPH in SCHEMATIC and BOARD 1-1-1c files.
* R25 = 2.7k (not 4.7k) - Compromised. R25 will show 4.7k for NTSC and 2.7k for PAL. 19 OCT, SPH in SCHEMATIC and BOARD 1-1-1c files.
* Tracks from PSU -> switch ->7805 very thin - Resolved by making sure all power nets were 32 mil from input to GND, to pure VCC, VPP, and VEE. Resolved 18 OCT 2020, SPH in SCHEMATIC and BOARD 1-1-1c files.
* Jumper (open - PAL/close - NTSC) between U11 Pin 12 and U6 Pin 2 (PCB is drilled to break the track on PAL version) - Added two jumper posts next to C25 (between U11 and U15). NTSC must bridge this to pass 2Φ signal to U11 pin 12. Resolved 18 OCT 2020, SPH in SCHEMATIC and BOARD 1-1-1c files.
* C38 = 100pf not 0.1uf as described - Resolved 18 OCT 2020, SPH in SCHEMATIC and BOARD 1-1-1c files.
* R49 - Goes to Via Below (+5V), for PAL, not the stated Hole (GND) (seems R49 has 2 holes!) - True. I didn't notice this until you mentioned it. NTSC grounds U7 PLA1 pin 13. PAL goes through 220 resistor to VCC. Resolved 18 OCT 2020, SPH in SCHEMATIC and BOARD 1-1-1c files.
* R13 - Via very close - Resolved 18 OCT 2020, SPH in BOARD 1-1-1c file. Note that this via is the same signal as the pin it was next to, so it wouldn't have been a problem.
* R52 = 100Ω - Resolved 18 OCT 2020, SPH in SCHEMATIC and BOARD 1-1-1c files.
* R50 = 1.5k - Resolved 18 OCT 2020, SPH in SCHEMATIC and BOARD 1-1-1c files.
* R51 = 1.5k - Resolved 18 OCT 2020, SPH in SCHEMATIC and BOARD 1-1-1c files.
* Pin 21 U5 needs to go to +5v - Resolved 18 OCT 2020, SPH in SCHEMATIC and BOARD 1-1-1c files.
* AUX power pin header needed - Resolved 10 SEP 2020, SPH in SCHEMATIC and BOARD 1-1-1c files.

## Delayed / Out of Scope
* ROM & CHROM 24 to 28 pin change - Deferred. It's impractical to add on-board support for both 24 pin (stock) and 28 pin (modern replacement) headers. 21 OCT 2020, SPH.
