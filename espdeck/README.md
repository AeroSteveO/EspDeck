# EspDeck

This is a StreamDeck inspired macro pad powered by EspHome for use with Home Assistant. Each key has 3 different actions it can perform, single click, double click, and click + hold. These can all be tied to different automations in Home Assistant. This project is made for ESPHome (hardware + ESPHome Configuration).

[![Made for ESPHome](/assets/images/made-for-esphome-black-on-white.svg)](https://esphome.io/guides/made_for_esphome.html)


# Functionality
ESPDeck provides a macropad type input set to Home Assistant based on ESPHome. This includes 3 modes of input for each keyswitch. 

  * Single Click
  * Double Click
  * Click and Hold

See also the previous generation EspDecks ([Gen 1](GEN1_README.md), [Gen 2](GEN2_README.md)) in this repository.

# Hardware Used
  * 1 x ESP8266 / NodeMCU
  * 9 x Relegendable KeyCaps (waterslide decal paper can also be used with existing keycaps, especially blank ones)
  * 9 x Mechanical key switches
  * Hot Glue
  * 3d printer material
  * various wire

# Case

Case design based off of: https://www.thingiverse.com/thing:5204033. I extended the height of the case for my inefficient use of space inside of it, I also made some modifications to better hold the Esp8266. The top of the case is currently press fit or hot glued on, though I'll be working on making it a screw in place top in the future.

Case design can also be found here: https://www.thingiverse.com/thing:5223223

# Wiring
The wiring is simple enough, we make use of the matrix keypad feature and wire the columns and rows to inputs on the ESP. We avoid GPIO15 as it doesn't have an internal pullup as well, simplifying our wiring.

![Third Generation Circuit Diagram](/assets/images/circuit-gen3.svg)

# Configuration

keypad3.yaml

# Printing Instructions
Print one each of:
  * MacroPadBottomExtended.stl
  * MacroPadTop.stl

These can be printed with low infill for speed.

# Contributing
Contributions are welcome to the project

# Change Log

  * With generation 3, we begin to use the Matrix Keypad feature of EspHome, simplifying the wiring.
  * With generation 4, we'll be adding WS2812 LEDs to backlight the key switches, providing an aveneue for notifying of a status from home assistant