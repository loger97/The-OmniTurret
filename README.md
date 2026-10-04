# The-OmniTurret
> **Credit to discord user [MrBanana](https://discord.com/users/1245929364265111674) for making this hack (I'm just fixing some problems)**

This makes your IR turret fully mobile. Now unlike some other "turret-tank" style hacks, this one requires no 3D printer, only 8 wires. (Oh, and some tape). 

## Materials
- Your completed IR Turret
- Your completed Omnibot
- 6 M-F jumper wires
- 2 M-M jumper wires
- Tape (Super 88 scotch tape or gaffe tape)

## Instructions
### Structural:
1. Remove the legs from your IR turret.
   - You can do this easily by unscrewing the bottom platform from the servo mount
   - Then taking off the orange hex nuts, removing the legs, and putting the bottom plate back on the servo mount.
3. Grab some tape. It can be any tape you want.
   - Tear 4 thin strips and use those to anchor your turret to the top plate of the Omnibot. That's literally it for building instructions.

### Wiring:
1. Unplug the 4-wire bundle of signal wires (the blue, green, yellow, and purple ones) from the turret.
2. Extend the connections for the Roll #3 and Pitch #2 servo motors using the 6 M-F jumper wires.
3. Connect the red and black wire bundles to the red and black rails on the Omnibot breadboard to connect power to the servos.
4. Connect the roll servo wire to pin 10 (next to the green and blue wires)
5. Connect the pitch servo to pin 13 (directly opposite that) using the two M-M wires.

**That's it for wiring!**

### Code:
> Use Github desktop to clone this repo on to your computer.
#### Option 1 - Arduino IDE
- Open the .ino file in Arduino IDE.
   - The IDE may prompt you to put it into a folder of the same name. Then drag config.h into that folder if it is not already there.
- Plug the micro controller into your computer, it may come up as "Unknown device (COM#)", select that.

#### Option 2 - CLIDE (not recommended, use only if you can't use Arduino IDE)
- Open CLIDE as OmniBot.
- Copy the contents of the .ino file to stockcode.ino in CLIDE.
- Copy the contents of config.h file to config.h in CLIDE.
- Plug the micro controller into your computer, it should come up as "Crunch labs Micro (COM#)", select that.

> Upload the code to the microcontroller.
