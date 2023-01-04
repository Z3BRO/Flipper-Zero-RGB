# Flipper-Zero-RBG-Backlight

Big thanks to Quenon#1989 and axum#6461 for making this possible!


Here is a Tutorial made by t.me/hitriy https://telegra.ph/Flipper-Zero-RGB-backlight-guide-12-26

Another Tutorial on how to remove the led backlight board (not 100% sure who made it) https://telegra.ph/Izmenenie-cveta-podsvetki-Flipper-Zero-11-14 you will need to translate it unless you speak russian


# Here are the links to everything you will need!


Capacitors - https://www.digikey.com/en/products/detail/kyocera-avx/06036C104JAT2A/1600414


Leds, Pack of 10 - https://www.digikey.com/en/products/detail/adafruit-industries-llc/4492/11569136

Thin gauge wire (im using 28 gauge bc its what i had) - https://shorturl.at/vBLY6

# Firmware stuff

All of the repos below have been modified with their respective patches

Unleashed - https://github.com/Z3BRO/unleashed-firmware/tree/RGB

OFW - https://github.com/quen0n/flipperzero-firmware-rgb/commits/release

# How to compile from the repos above 

Step 1: git clone --recursive FIRMWARELINKFROMABOVE


Step 2: git switch RGB


Step 3: ./fbt updater_package


Step 4: Navigate to dist\f7-D\ in the cloned repos folder ( Usually found at Documents\GitHub)


Step 5: Copy the f7-update-local folder to the Update folder on your Flipper


Step 6: On your Flipper Navigate to the Update folder


Step 7: Open the f7-update-local folder


Step 8: Update from the update.fuf file  ( It will have a picture of a box with an arrow next to it)


# How to update from the pre compiled firmware

Step 1: git clone --recursive https://github.com/Z3BRO/Flipper-Zero-RBG-Backlight


Step 2: Navigate to the cloned repo ( usually its Documents\GitHub\Flipper-Zero-RBG-Backlight)


Step 3: Open the Update Files folder


Step 4: Copy the desired folder to the Update Folder on your Flipper


Step 5: On your Flipper Navigate to the Update folder


Step 6: Open the folder you just added ( Either OFW-0.74.2-RGB or Unleashed22-RGB)


Step 7: Update from the update.fuf file  ( It will have a picture of a box with an arrow next to it)





# Notes

When purchasing the pcb make sure to have the thickness set to 0.6mm and the layer ammount set as 2.

Here is a video on how to use git patch files https://www.youtube.com/watch?v=ArbQNoNlFXk
