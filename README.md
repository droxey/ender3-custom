# ender3-custom

[@droxey](https://github.com/droxey)'s **customized TH3D firmware for the Ender3**.

## Firmware Features

* Disabled buzzer when using the LCD.
* Added `DROXEYBOT` as the printer name.

## Development

Download the [TH3D Unified Firmware Package](https://www.th3dstudio.com/knowledge-base/th3d-unified-firmware/) to create your own customized firmware. This repository initially started with the aformentioned base package, applying additional Ender3 settings for daily usage.

### Hardware Setup

1. Wire up the 5 male-to-male and 1 male-to-female dupont cables that facilitate the connection between the 3D printer motherboard and the Arduino UNO.
1. Plug in Arduino UNO via USB.
1. Open the Arduino IDE.
1. Go to **`File` > `Examples` > `Arduino ISP` > `Arduino ISP`**. A new sketch and it's corresponding code will appear.
1. Upload this new `Arduino ISP` sketch to UNO. Use these settings:
    * **`Tools` > `Board`**: `Sanguino`
    * **`Tools` > `Processor`**: `ATMega1284 or ATMega1284p (16 MHz)`
    * **`Tools` > `Port`**: `Arduino Uno`
    * **`Tools` > `Programmer`**: `Arduino as ISP`
1. Run **`Tools` > `Burn Bootloader`** to complete the **one-time Arduino UNO setup!**

### Making Changes

1. Connect the 3D printer's motherboard to the UNO.
1. Open the [`firmware/TH3DUF_R2/TH3DUF_R2.ino`](firmware/TH3DUF_R2/TH3DUF_R2.ino) sketch in the Arduino IDE.
1. Make changes to various `#define` statements to tweak your settings.
1. Verify and Upload sketch to Arduino UNO to test.
1. Add, commit, and push changes to GitHub.


