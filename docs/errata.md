# Errata
Updated 19 OCT 2020, by Mack Wharton
Updated 18 OCT 2020, by Sean Harrington

## New
* Pin 1 label on U13 against wrong pin (Pin 14)
## Feedback Needed
* C1 = 10uf - Both my PAL and my NTSC board show C1 (bottom center of FRONT) as 1uF @ 50v
* R25 = 2.7k (not 4.7k) - Both my PAL and my NTSC board show R15 (upper right of U7 PLA1) as 4.7k (YELLOW PURPLE RED GOLD)
* R15 = 2.2K (not 1.2k) - Both my PAL and my NTSC board show R15 (right of Q5) as 1.2k (BROWN RED RED GOLD)
* R14 = 680R (not 2.2K) - Both my PAL and my NTSC board show R14 (between U10 and Q5) as 2.2k (RED RED RED GOLD)

## Resolved
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
* None
