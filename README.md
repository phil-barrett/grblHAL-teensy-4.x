# grbl-teensy-4
GRBL Breakout Boards for Teensy 4.x Uses the [grblHAL Teensy 4 version](https://github.com/terjeio/grblHAL).

# Resources for grblHAL, T41U5XBB and related CNC topics
[Resources](https://www.grbl.org/resources)

## Aug 20, 2025.  V2.10 is now available.
Trimmer potentiometer moved onto PCB, unneeded features removed and some cosmetic changes.  Now using KiCAD instead of Eagle. V2.11 is coming but is functionally the same as V2.10 (minor slik screen changes).  [User Manual](https://github.com/phil-barrett/grblHAL-teensy-4.x/blob/master/T41U5XBB%20User%20Manual.pdf) updated. 


## Oct 15, 2020.  V2.09 is now available.
A small number of changes, mostly cosmetic. Also added mounting holes for I2C and Serial I/O daughter boards. [Now available on Tindie.](https://www.tindie.com/products/philba/grblhal-breakout-board-unkit-for-teensy-41/) 
![T4.1 BreakuoutBoard](https://github.com/phil-barrett/grbl-teensy-4/blob/master/RA159231_DxO_2048.jpg "V2.09 Unkit PCB")

## Sept 29, 2020. Ethernet Support Added
grblHAL support for Ethernet is now pretty solid.  I have updated the [User Manual](https://github.com/phil-barrett/grblHAL-teensy-4.x/blob/master/T41U5XBB%20v207.pdf) to include instructions on using Ethernet. 

## June 28, 2020. New Versions!
I have finished 2 new 5 axis versions based on the Teensy 4.1. One supports an Ethernet interface and the other supports a USB interface. I will be making a few "Unkit" boards avalable. These have all the surface mount components installed (with the execption of the EEPROM IC). Teensy 4.1 not included. The price is $27.99 USD. [It is available on Tindie.](https://www.tindie.com/products/philba/grblhal-breakout-board-unkit-for-teensy-41/)  There are a limited number but if there is enough interest, I will reorder more.

The "Unkit" board.
![T4.1 BreakuoutBoard](https://github.com/phil-barrett/grbl-teensy-4/blob/master/R6288808_DxO.jpg "Unkit Version")
T41U5XBB - Fully populated USB based version.  
![T4.1 BreakoutBoard](https://github.com/phil-barrett/grbl-teensy-4/blob/master/R6278732_DxO.jpg?raw=true "T4.1 USB Breakout Board - T41U5XBB")

T41E5XBB - Fully populated Ethernet version
![T4.1 BreakoutBoard](https://github.com/phil-barrett/grbl-teensy-4/blob/master/R6278738_DxO.jpg?raw=true "T4.1 Ethernet BreakoutBoard - T41E5XBB")

Lots of new features!
## Features
  * 5 Axis control outputs – 5V compatible.
  * Independent enables for each axis.
  * 10 Opto-isolated inputs including standard GRBL controls and limits switches for all axes.
  * 7 Relay Outputs – Spindle, Mist Coolant, Flood Coolant, Dust Collector and 3 auxiliary relays. Each output can control a relay coil directly or 5V TTL (SSR compatible) devices.
  * Dust Extraction relay support. Activated by spindle enable.
  * Separate control of Dust Collector relay via pin header.
  * Relay coil voltage switchable between 5V and 12V. 
  * Standard GRBL spindle control outputs – 5V compliant.
  * 0-10V spindle control output.
  * Screw Terminals for reliable connections available for most I/O.
  * 4 Digital Inputs – EMI protected, 15.9KHz low pass filter, Schmitt Trigger.
  * I2C header.
  * EEPROM footprint for SOIC8 devices.
  * LED indicators for 5V and 12V.
  * USB interface.
  * Ethernet interface. (T41E5XBB only)
  * Serial I/O Header

## Firmware
Prebuilt versions of grblHAL are available to directly load into the Teensy 4.1 [Follow the instructions here.](https://github.com/phil-barrett/grblHAL-teensy-4.x/blob/master/prebuilt.md)

## Documentation
### Schematic
The two versions currently share a common schematic and PCB layout. This may not be the case in the future. [Schematic is here.](https://github.com/phil-barrett/grbl-teensy-4/blob/master/v2.07%20schematic.pdf)

### Manual
The [User Manual is available here.](https://github.com/phil-barrett/grbl-teensy-4/blob/master/T41U5XBB%20v207.pdf)

### Bare PCB from OSHPark
[Available here](https://oshpark.com/shared_projects/QWr3OZUe) This is fairly expensive. For a less costly approach, you can use the Gerber files below to order from more cost effective fabs.

### Gerbers
[Gerbers are available here.](https://github.com/phil-barrett/grbl-teensy-4/blob/master/teensy%204.1x207.zip) Board size is 85 x 96 mm, 2 layer, 1.6 mm thickness.

### Build Guide
A brief guide to building grblHAL from source [for the breakout board is here](https://github.com/phil-barrett/grbl-teensy-4/blob/master/grblHAL%20Build%20Guide.pdf).

## Previous Version
![T4 Breakout Board](https://github.com/phil-barrett/grbl-teensy-4/blob/master/PCB%20V100.jpg?raw=true "T4 Breakout Board")

## Features:
  * 4 Axis control outputs – 5V Compatible.
  * 8 Opto-isolated inputs.
  * Full spindle control outputs – 5V compatible.
  * 0-10V spindle control output.
  * 7 Relay Outputs.
  * Relay voltage switchable between 5V and 12V. 
  * Dust Extraction relay output slaved to spindle.
  * Screw Terminal I/O for reliable connections.
  * I2C header.
  * EEPROM footprint for SOIC8 devices.
  * LED indicators for 5V and 12V.
