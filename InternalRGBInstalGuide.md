# Prerequisite

This guide will start at the point where your original orange backlight is removed from your Flipper. You can use [This Guide](https://telegra.ph/Izmenenie-cveta-podsvetki-Flipper-Zero-11-14) (Needs translation if you don't speak Russian), [This Guide](https://telegra.ph/Flipper-Zero-RGB-backlight-guide-12-26) or [This Video Guide](https://www.youtube.com/watch?v=pft1CI5ikA4) to get to that point.

If you're just installing the RGB Backlight, skip all steps necessary for Internal RGB and only solder a wire to the Data-In pad on the RGB Backlight.

# For this installation you will need

- Flipper Zero
- PH #0 Screwdriver
- ~1mm Flathead Screwdriver 
- Soldering Iron
  - Solder and Flux
- Some thin wire (I like using [UL10064 36ga insulated wire](https://www.aliexpress.us/item/3256805268543019.html) from AliExpress)
- Double-sided adhesive under 4mm thick (I used some random 3mm stuff that I had laying around)
- RGB Backlight with a Data-Out Pad
- Internal RGB Flex PCB

![image00001](https://github.com/Z3BRO/Flipper-Zero-RGB/assets/101530102/3559a438-ee9c-4344-a2e8-0555d2a26aa7)

# The Install

Cut two lengths of your wire, one about double the length of the other. Keep them longer than needed; you can always trim them later. Solder the longer length of wire to the Data-Out Pad on your backlight and the shorter one to the Data-In Pad on the backlight.

![Out](https://github.com/Z3BRO/Flipper-Zero-RGB/assets/101530102/51a60c4d-59ef-40d4-ac59-9e6a71cafeec)

Place the Backlight into the LCD like so; make sure to reinstall the reflector on the back of the LCD; otherwise, you'll have a very bad time.

![image00003](https://github.com/Z3BRO/Flipper-Zero-RGB/assets/101530102/0fb46f54-6331-4568-bf47-ddafb05bc6cd)

Now, reinstall the LCD Assembly. Make sure you route the data wires under the LCD Flex Connector and to the left.

![image00019](https://github.com/Z3BRO/Flipper-Zero-RGB/assets/101530102/cd77e51a-0b2f-492e-8a9d-7e5edb338fd4)

Solder the backlight to the Flipper's Main PCB, use lots of flux during this process. 

![image00004](https://github.com/Z3BRO/Flipper-Zero-RGB/assets/101530102/0ecb3535-cad1-4c99-91e4-aea7741e1425)

Since the "ground" pad for the backlight on the Main PCB isn't really a ground point, solder a wire from the left pad to the GND3 test point.

![Untitled design](https://github.com/Z3BRO/Flipper-Zero-RGB/assets/101530102/ffb5ac32-d1e3-4a42-b0da-7464786de9b1)

Take the shorter data wire (Data-In) and solder it to the VIBRO test pad. Be careful as that pad is very close to a GPIO header and some capacitors.

![Untitled design (1)](https://github.com/Z3BRO/Flipper-Zero-RGB/assets/101530102/e676c9b3-ea12-4c75-9d1d-22668eda3c48)

This would be a good time to connect the battery and test that the RGB Backlight works. If everything is good, you can reinstall the Black plastic that holds the buttons and LCD in place. 

Route the remaining data wire like shown, pulling it underneath the Data-In wire.

![image00008](https://github.com/Z3BRO/Flipper-Zero-RGB/assets/101530102/4d764116-e9de-48e7-9669-ec9c0eb0d04f)

Now, you can start reassembling the Flipper and snap the Main PCB Assembly to the rest of the Flipper's internals. The Data-Out wire should be on top of the USB-C port, as shown below. 

![image00009](https://github.com/Z3BRO/Flipper-Zero-RGB/assets/101530102/27b00f4e-7fa5-4170-b7be-1d414f20ddba)

It is time to start bending the Internal RGB PCB and applying the adhesive. Apply a thin strip of double-sided tape to the back of LED 1 and make bends along the dotted lines shown below.

![Double-sided Tape here](https://github.com/Z3BRO/Flipper-Zero-RGB/assets/101530102/240c4874-2f14-48fd-838c-e5ad9cd41b4e)

After making all the necessary bends, compare your Internal RGB PCB to the one below.

![image00013](https://github.com/Z3BRO/Flipper-Zero-RGB/assets/101530102/082a24cc-85e9-4280-97ba-54850f819e81)

If everything looks good, remove the backing on the double-sided tape and place the Internal RGB PCB on the flipper, as shown below. Make sure you line up all of the holes on the Internal RGB PCB with the test pads on the NFC/RFID PCB.

![image00014](https://github.com/Z3BRO/Flipper-Zero-RGB/assets/101530102/a31ec6bb-eda1-4925-b5e7-bb4f100250b1)

![image00015](https://github.com/Z3BRO/Flipper-Zero-RGB/assets/101530102/3dfdcb28-e715-4393-bf4e-a8d5c7174322)

If everything lines up, liberally apply flux and solder the 5V, GND, and two anchors to the Flippers NFC/RFID PCB. Next, bring the remaining data wire over the Vibro motor and solder it to the Internal RGB PCB. Finally, you can reinstall the iButton PCB.

![Untitled design (3)](https://github.com/Z3BRO/Flipper-Zero-RGB/assets/101530102/47a250e7-7377-432c-aa1a-3e121695f348)

Now its time to test that everything is working correctly before putting it back in the shell. Reconnect the battery and plug your sd card in, then flash [OFW (With Internal RGB Support)](https://github.com/Z3BRO/Flipper-Zero-OFW-RGB) to your Flipper. Go through the RGB Settings page in the setting app and make sure everything is working. If it is, then you can disconnect the battery and sd card, then continue with the guide.

Be careful when inserting the Flipper into the top shell. It's very easy to rip the LEDs off their pads. The single LED between the two GPIO headers should go completely into the top shell, while the strip of 6 LEDs will have some sticking out. 

![image00018](https://github.com/Z3BRO/Flipper-Zero-RGB/assets/101530102/3c2d9d01-0420-46bb-9407-fba8e3143a09)

![image00017](https://github.com/Z3BRO/Flipper-Zero-RGB/assets/101530102/c6208926-cb14-4d34-b6d1-0696058c3477)

Now its time to put the bottom shell on; in my experience, it is easiest to start with the side with 6 LEDs, and then clip the other side in. When putting the bottom shell on it WILL rip the LEDs off their pads if you are not careful. Take your small Flathead screwdriver and use it to push LEDs 1, 2, and 6 underneath the bottom shell. Take your time with this process, if you do it wrong you're screwed.

![1 2 3 4 5 6](https://github.com/Z3BRO/Flipper-Zero-RGB/assets/101530102/0c0f6b23-80d3-422b-89db-967485620779)

Once all the LEDs are under the bottom shell, you can clip the bottom shell into place, and that's it! Go and test all the LEDs BEFORE screwing in the bottom shell.

YAYAYAYAYAYAYAY. You are now the proud owner of a blindly bright RGB Flipper Zero, be sure to make fun of all your hacker friends who don't have an RGB Fliper because I'm poor and need people to buy my mod.


