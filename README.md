# ender3-firmware

[@droxey](https://github.com/droxey)'s **customized TH3D firmware for the Ender3**.

## Features

* Disabled buzzer when using the LCD.
* Added `DROXEYBOT` as the printer name.

## Prerequisites

* Guide written for `Ardunio v1.8.5` which is part of the [TH3D Unified Firmware Package](https://www.th3dstudio.com/knowledge-base/th3d-unified-firmware/). This repository starts with this downloaded base package, applying additional, helpful Ender3 settings for daily usage.

## Development

### Hardware Setup

* Wire up the 5 male-to-male and 1 male-to-female dupont cables that facilitate the connection between the 3D printer motherboard and the Arduino UNO.
* Plug in Arduino UNO via USB.
* Open the Arduino IDE.
* Go to `File` > `Examples` > `Arduino ISP` > `Arduino ISP`. A new sketch and it's corresponding code will appear.
* Upload this new `Arduino ISP` sketch to UNO. Use these settings:
  * **`Tools` > `Board`**: `Sanguino`
  * **`Tools` > `Processor`**: `ATMega1284 or ATMega1284p (16 MHz)`
  * **`Tools` > `Port`**: `Arduino Uno`
  * **`Tools` > `Programmer`**: `Arduino as ISP`
* Run **`Tools` > `Burn Bootloader`** to complete the **one-time Arduino UNO setup!**

### Making Changes

* Connect the 3D printer's motherboard to the UNO.
* Open the [TH3DUF_R2/TH3DUF_R2.ino](TH3DUF_R2/TH3DUF_R2.ino) sketch in the Arduino IDE.
* Make changes to various `#define` statements to tweak your settings.
* Verify and Upload sketch to Arduino UNO to test.
* Add, commit, and push changes to GitHub.
