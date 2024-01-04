# EspDeck

This is a StreamDeck inspired macro pad powered by EspHome for use with Home Assistant. Each key has 3 different actions it can perform, single click, double click, and click + hold. These can all be tied to different automations in Home Assistant. This project is made for ESPHome (hardware + ESPHome Configuration).

[![Made for ESPHome](/assets/images/made-for-esphome-black-on-white.svg)](https://esphome.io/guides/made_for_esphome.html)


# Functionality
ESPDeck provides a macropad type input set to Home Assistant based on ESPHome. This includes 3 modes of input for each keyswitch. 

  * Single Click
  * Double Click
  * Click and Hold

See also the ![Novelkey Novelty Big Switch Macropad](/novelkey-big-switch/README.md) and the [Gen 1 EspDeck](GEN1_README.md) is also documented.

# Hardware Used
  * 1 x ESP8266 / NodeMCU
  * 9 x Relegendable KeyCaps (waterslide decal paper can also be used with existing keycaps, especially blank ones)
  * 9 x Mechanical key switches
  * 1 x 10k Resistor
  * Hot Glue
  * 3d printer material
  * various wire

# Case

Case design based off of: https://www.thingiverse.com/thing:5204033. I extended the height of the case for my inefficient use of space inside of it, I also made some modifications to better hold the Esp8266. The top of the case is currently press fit or hot glued on, though I'll be working on making it a screw in place top in the future.

Case design can also be found here: https://www.thingiverse.com/thing:5223223

# Wiring
The wiring is simple enough, one end of the switch going to the digitial IO pin, and the other end to ground, and set up ESPHome to have the internal pullup enabled on the ESP8266 device. Two of the GPIOs on the device cannot be done this way, GPIO16 needs an external pullup resistor, and GPIO15 needs to be inverted (internal pulldown, external pullup).

![Second Generation Circuit Diagram](/assets/images/circuit-gen2-full.svg)


![Second Generation Circuit Diagram Simplified](/assets/images/circuit-gen2-simplified.svg)

# Configuration

keypad2.yaml

# Printing Instructions
Print one each of:
  * MacroPadBottomExtended.stl
  * MacroPadTop.stl

These can be printed with low infill for speed.

# Contributing
Contributions are welcome to the project

