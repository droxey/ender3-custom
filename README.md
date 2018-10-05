# ender3-custom

[@droxey](https://github.com/droxey)'s **customized TH3D firmware for the Ender3**.

## Features

### Cura

* [PLA - 0.4mm-0.1mm](cura/configurations/PLA_0.4mm-0.1mm.curaprofile)
* [PLA - 0.4mm-0.2mm](cura/configurations/PLA_0.4mm-0.2mm.curaprofile)

### Firmware

* Disabled buzzer when using the LCD.
* Added `DROXEYBOT` as the printer name.

## Development

Download the [TH3D Unified Firmware Package](https://www.th3dstudio.com/knowledge-base/th3d-unified-firmware/) to create your own customized firmware. This repository initially started with the aformentioned base package, applying additional Ender3 settings for daily usage.

### Hardware Setup

* Wire up the 5 male-to-male and 1 male-to-female dupont cables that facilitate the connection between the 3D printer motherboard and the Arduino UNO.
* Plug in Arduino UNO via USB.
* Open the Arduino IDE.
* Go to **`File` > `Examples` > `Arduino ISP` > `Arduino ISP`**. A new sketch and it's corresponding code will appear.
* Upload this new `Arduino ISP` sketch to UNO. Use these settings:
  * **`Tools` > `Board`**: `Sanguino`
  * **`Tools` > `Processor`**: `ATMega1284 or ATMega1284p (16 MHz)`
  * **`Tools` > `Port`**: `Arduino Uno`
  * **`Tools` > `Programmer`**: `Arduino as ISP`
* Run **`Tools` > `Burn Bootloader`** to complete the **one-time Arduino UNO setup!**

### Making Changes

* Connect the 3D printer's motherboard to the UNO.
* Open the [`firmware/TH3DUF_R2/TH3DUF_R2.ino`](firmware/TH3DUF_R2/TH3DUF_R2.ino) sketch in the Arduino IDE.
* Make changes to various `#define` statements to tweak your settings.
* Verify and Upload sketch to Arduino UNO to test.
* Add, commit, and push changes to GitHub.


