# Errata
Updated 18 OCT 2020, by Sean Harrington

## New
* R50 = 1K5
* R51 = 1K5
* R52 = 100Ω 
* R14 = 680R (not 2.2K)
* R15 = 2.2K (not 1.2k)
* R25 = 2.7k (not 4.7k)
* R13 - Via very close
* R49 - Goes to Via Below (+5V), for PAL, not the stated Hole (GND) (seems R49 has 2 holes!)
* C38 = 100pf not 0.1uf as described
* C1 = 10uf 
* Tracks from PSU -> switch ->7805 very thin
* Jumper (open - PAL/close - NTSC) between U11 Pin 12 and U6 Pin 2 (PCB is drilled to break the track on PAL version)

## Resolved
* Pin 21 U5 needs to go to +5v - Resolved 18 OCT 2020, SPH in SCHEMATIC and BOARD 1-1-1c files.
* AUX power pin header needed - Resolved 10 SEP 2020, SPH in SCHEMATIC and BOARD 1-1-1c files.

## Delayed / Out of Scope
* None, yet.
