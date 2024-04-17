 ![Flipper Zero RGB](https://user-images.githubusercontent.com/89728480/226134250-966746b9-74c1-461a-a6d4-82453af41d7c.gif)

# Flipper Zero RGB

    Big thanks to Quenon#1989, t.me/hitriy, axum#6461, and codeallnight#1337 for making this possible!
This repo is the complilation of all the information avaliable on the Flipper Zero RGB Mods.
# RGB Backlight
Here you can find all the information on the RGB Backlight Mod for the Flipper Zero

## Showcase Video 
- [YouTube](https://youtu.be/W1frMyVFv6Y)
## RGB Backlight Parts

- Capacitors (0.1uF 0603):
  - [Digikey](https://www.digikey.com/en/products/detail/kyocera-avx/06036C104JAT2A/1600414)
- LEDs (SK6805-EC 15):
  - [Digikey](https://www.digikey.com/en/products/detail/adafruit-industries-llc/4492/11569136)
  - [Adafruit](https://www.adafruit.com/product/4492)
  - [Mouser](https://mouser.com/ProductDetail/Adafruit/4492?qs=CUBnOrq4ZJz3oeplDXDOWA%3D%3D)
  - [AliExpress](https://www.aliexpress.us/item/2251832771718100.html)
- Thin gauge wire (36 AWG):
  - [AliExpress](https://www.aliexpress.us/item/3256805268543019.html)

For each Module, you need 3 Capacitors and 3 LEDs

When purchasing Backlight PCBs, ensure the thickness is set to 0.6mm and the layer amount is set to 2.

## RGB Backlight Build Guides

- [Video Guide by Z3BRO](https://youtu.be/pft1CI5ikA4)
- [Guide by t.me/hitriy](https://telegra.ph/Flipper-Zero-RGB-backlight-guide-12-26)
- [LED Backlight Board Removal Tutorial (Russian)](https://telegra.ph/Izmenenie-cveta-podsvetki-Flipper-Zero-11-14) - Translation may be needed.

## RGB Backlight PCB Assembly

- [Assembly Video](https://youtu.be/N64fDjziTaE)

# Internal RGB
Internal RGB For the Flipper Zero is a mod I have been working on for about a year now.

This mod is for people with a Transparent/Translucent Shell that want their Flippers to be a glowing beacon of light for the Flipper Gods, or they just wanna let you know that their Flipper is cooler than yours because it has gamer lights.

## Where to purchase
For now, the Internal RGB Mod is going to be sold exclusively on [Rabbit-Labs.com](https://rabbit-labs.com). I plan to release the board for sale by the end of this month (but it will probably be early next month)

## Supporting Mods
The first batch of Internal RGB Mods will require the user to solder a wire to a Vibro test pad or to the Data Out pad of RGB Backlights that have it (Not all RGB Backlights have a Data Out pad, those that do not are not compatiable with Internal RGB). 

After I placed the order for a production run of Internal RGB I noticed there was a Vibro test pad on the RFID/NFC PCB underneath the mod, on future releases of Internal RGB you will have to option to do a completley wireless install (you will still have to solder the Internal RGB PCB to the RFID/NFC PCB, you just wont need any wires). 

Please note that if you would like to use an RGB Backlight along side your Internal RGB you MUST solder a wire from the RGB Backlight's Data Out pad to the Internal RGB's Data In pad, connecting both the RGB Backlight and Internal RGB to the Vibro line WILL result in issues when changing the color of the LEDs.

## How to install
I will have a written guide as well as a video guide on the instalation process done shortly.

# Supported Firmwares

All repositories below support the RGB Backlight Mod. Only the community modified OFW Supports Internal RGB as of right now.

- **Community Modified**:
  - [OFW (With Internal RGB Support!)](https://github.com/Z3BRO/Flipper-Zero-OFW-RGB)

- **Natively Supported**:
  - [Momentum Firmware](https://github.com/Next-Flip/Momentum-Firmware)
  - [Unleashed Firmware (RGB Specific Build)](https://github.com/DarkFlippers/unleashed-firmware)
  - [RougeMaster Firmware](https://github.com/RogueMaster/flipperzero-firmware-wPlugins)
  - [Xtreme Firmware](https://github.com/Flipper-XFW/Xtreme-Firmware)
  
Shield: [![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]

This work is licensed under a
[Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License][cc-by-nc-sa].

[![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]

[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg
