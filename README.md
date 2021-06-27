# AEK II USB

[![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]

#### QMK compatible drop-in replacement PCB for the Apple Extended Keyboard II - Now featuring Teensy++ 2.0!
The PCB is built entirely with THT parts to keep a somewhat "vintage" look to it and it uses a 40-pin Teensy++ 2.0, mounted in a socket.
The controller is placed in the exact same location as the one on the original PCB.

This is a trivial fork of the original aek2_usb by kb-elmo: https://github.com/kb-elmo/aek2_usb. All credit to Elmo for his original work! I've just edited it a bit.

This version simplifies the design and adds additional power (and RAM) by relying on a Teensy++ 2.0 to handle all USB operations and run the firmware.

### Partslist
Most of the parts in this list are just examples and they can be replaced with any component with the same specs.  
They don't have to be from any specific manufacturer or brand to work on this board.

The USB breakout PCB/Daughterboard is NOT included in this repo. You will have to find one yourself.  
Pretty much any kind of breakout board that has usable VCC, GND, D+ and D- pins should work for this.  
Example: https://www.adafruit.com/product/1764

|Count|Part|Designator|URL|
|-|-|-|-|
|1|Teensy++ 2.0 microcontroller|U1|[Atmega32a-pu](https://www.pjrc.com/store/teensypp.html)|
|1|40 pin DIP socket (optional but highly recommended)|U1|[TE Connectivity 1-2199299-5](https://octopart.com/1-2199299-5-te+connectivity-34963610)|
|3|JST PH 2mm 4pin connector + cable|J1, J2, J3|[JST S4B-PH-K-S](https://octopart.com/s4b-ph-k-s+%28lf%29%28sn%29-jst-5373077)|
|1|USB breakout PCB||[Adafruit 1833](https://octopart.com/1833-adafruit+industries-53099556)|
|3|5mm LED (for the lock indicators)|LED1, LED2, LED3|[Vishay TLHG5400](https://octopart.com/tlhg5400-vishay-39403037)|
|105|universal switching diode (DO-35 1N4148)|D3-D107|[ON Semiconductor 1N4148](https://octopart.com/1n4148-on+semiconductor-6807167)|

---
This work is licensed under a
[Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License][cc-by-nc-sa].

[![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]

[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg
