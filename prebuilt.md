## Prebuilt Firmware

### Prebuilt Firmware depreciated
With advent of the Web Builder, it is very easy to build custom versions of grblHAL firmware.  As such, there is no need for prebuilt versions. We will leave the current files available but highly recommend moving to the [grblHAL Web Builder](http://svn.io-engineering.com:8080/). For more information, take a look at a brief [tutorial on the grblHAL Web Builder](https://www.grbl.org/single-post/using-the-grblhal-web-builder).


### Using the Web Builder
Some Web Builder configuration files are [located here](https://github.com/phil-barrett/grblHAL-teensy-4.x/blob/master/iMXRT1062_T41U5XBB-files.zip). Download and extract the file that reflects your machine. Use the Load Board button to load the .json file. If one does not meet you exact needs, choose the one that is closest and modify it.

Here are the configuration files that are available:
iMXRT1062_T41U5XBB-3X.json - 3 Axis

iMXRT1062_T41U5XBB-3X-qangY.json - 3 Axis, Gang Y

iMXRT1062_T41U5XBB-3X-AutoSqY.json - 3 Axis, Auto-Square Y

iMXRT1062_T41U5XBB-3X-AutoSqY-SDCard-Keypad.json - 3 Axis, Auto Square Y, SDCard, Keypad

iMXRT1062_T41U5XBB-4X.json - 4 Axis

iMXRT1062_T41U5XBB-4X gangY.json - 4 Axis, Gang Y

iMXRT1062_T41U5XBB-4X-AutoSqY.json - 4 Axis, Auto-Square Y

iMXRT1062_T41U5XBB-4X-AutoSqY-SDCard-Keypad.json - 4 Axis, Auto-Square Y, SDCard, Keypad

iMXRT1062_T41U5XBB-5X-SDCard-Keypad.json - 5 Axis, SDCard, Keypad


Depreciated text follows.
### Available Versions
These are found in [configurations.zip](https://github.com/phil-barrett/grblHAL-teensy-4.x/blob/master/configurations.zip).   There are no USB only versions anymore.  These versions all work with USB or Ethernet. At this time, we do not recommend using the compat versions - you should use one of the many GCode Senders that work with grblHAL. If you need compatibility mode and other options, you will need to install the source from github and build it.

"3X qei" - 3 Axis, Aux Relays, Quadrature Encoder

"3X qangY qei" - 3 Axis, Aux Relays, Quadrature Encoder

"3X qangY AutoSq qei" - 3 Axis, Aux Relays, Quadrature Encoder

"3X qangY AutoSq qei SDCard Keypad" - 3 Axis, Aux Relays, Quadrature Encoder

"3X compat" - 3 Axis, no options, compatibility with older senders.

"4X qei" - 4 Axis, Aux Relays, Quadrature Encoder

"4X gangY qei" - 4 Axis, Aux Relays, Quadrature Encoder

"4X gangY AutoSq qei" - 4 Axis, Aux Relays, Quadrature Encoder

"4X gangY AutoSq qei SDCard Keypad" - 4 Axis, Aux Relays, Quadrature Encoder

"4X compat" - 4 Axis, no options, compatibility with older senders.

"5X qei SDCard Keypad" - 5 Axis, Aux Relays, Quadrature Encoder

"5X compat" - 5 Axis, no options, compatibility with older senders.


### Options
nX - number of axes

gangY - Y Motor is ganged with A (if 3 Axis) or B (if 4 Axis)

qei - Quadrature encoder on digital inputs. Supports spindle and feed rate override.

Compat - Sender compatibility.  disables new features of grblHAL and maintains compatibility with senders.

SDCard - SDCard support

Keypad - keypad support

More options will be added in the future.

### Loading Firmware onto a Teensy 4.1
Follow these basic steps:
1. Download the [firmware configurations file](https://github.com/phil-barrett/grblHAL-teensy-4.x/blob/master/configurations.zip) and extract the contents.
2. Select the .hex file that coresponds to the features you will use.
3. Obtain the Teensy Loader for your platform.
4. Use the loader to load the .hex file into your Teensy.

See the platform sections for details and hints.

#### Windows 
Download Teensy.exe from the [PJRC Website here](https://www.pjrc.com/teensy/loader_win10.html). The page may say Windows Vista but it works for all recent Windows versions.
Plug in your Teensy 4.1 via USB. Find Teensy.exe and run it.  It should open as a small window. In File/Open HEX File, select and open the .hex file you want and press OK. Then, press the button on the Teensy 4.1. You are ready to test it now. 

#### Macintosh OS X
Macintosh instructions [are here](https://www.pjrc.com/teensy/loader_mac.html). Plug in your Teensy 4.1 via USB. Follow the instructions to install and run the loader. It should open as a small window. Then, from the File name, choose "Open HEX File" and open the .hex file you want and press OK. Select "Program" from the "Operations" menu, or click the Program button on the tool bar. It should display a brief loading message. You are ready to test it now

#### Linux
Instructions for Ubuntu [are here](https://www.pjrc.com/teensy/loader_linux.html). Other Linux versions work though you will need to build the loader for your platform.  The [instructions and links to the github repository are here.](https://www.pjrc.com/teensy/loader_cli.html)
