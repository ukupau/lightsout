# lightsout
Lights out puzzle for the Altair 8800 front panel
(https://github.com/ukupau/lightsout)

## Description
This was an attempt to do something fun with the Altair front panel.
After doing some blinkenlights, I waa looking for a second project.
I found Steve Gibson's puzzle game that he wrote for his PDP 8 front panel.
My version was kept simple as I'm not that proficient at assembly and wanted to keep it within a 256 byte page.
As the Altair front panel is somewhat limited in its ability to interact with the user, it just makes use of the 8 leftmost
LEDs and switches.

## Assembling
This project was tested on an Altair-Duino replica and not a real Altair.
Although I believe it should work.

Assembly and compilation was done using asm80.com. 

It should be loaded at address 0 to avoid interfering with the upper 8 address bit LEDs.

## Rules of the game
The leftmost 8 LEDs of the address indicators will display a random pattern.

Each of the leftmost 8 address switches are each assigned 2 LEDs to toggle. 
Flipping a switch on will toggle the state of the 2 LEDs. 
If the LED is off, it will turn on. If it is on, it will turn off.

A specific pattern of on and off switches will turn off all the LEDs.

## Authors

* [Steven Chock](https://github.com/ukupau)

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Links

* Steve Gibson [Lights Out for the SBC6120/FP6120](https://www.grc.com/pdp-8/lightsout-sbc.htm)
* [asm80](https://www.asm80.com/) online assembler
* Altair-Duino [kit](https://www.altairduino.com/)