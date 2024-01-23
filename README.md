# EspDeck

This is a StreamDeck inspired macro pad powered by EspHome for use with Home Assistant. Each key has 3 different actions it can perform, single click, double click, and click + hold. These can all be tied to different automations in Home Assistant. This project is made for ESPHome (hardware + ESPHome Configuration).

[![Made for ESPHome](/assets/images/made-for-esphome-black-on-white.svg)](https://esphome.io/guides/made_for_esphome.html)


# Functionality
ESPDeck provides a macropad type input set to Home Assistant based on ESPHome. This includes 3 modes of input for each keyswitch. 

  * Single Click
  * Double Click
  * Click and Hold

# Variants
There are a number of variants of the device in this repository. The standard EspDeck is a 9 key pad. There is also the novelkey macropad, which has two BIG switches, and an upcoming design to add NFC functionality to the EspDeck macropad (NfcDeck). All of these use the same basic features in ESPHome and previous iterations of the designs are maintained for legacy support. Do look at the variant specific README files for the hardware needed, 3d print files, and yaml configurations.

## EspDeck
[![EspDeck](/assets/images/espdeck.jpg)](/espdeck/README.md)

There are also previous generation EspDecks ([Gen 1](/espdeck/GEN1_README.md), [Gen 2](/espdeck/GEN2_README.md)) in this repository.

## NfcDeck
[![NfcDeck](/assets/images/nfcdeck.jpg)](/nfcdeck/README.md)

### Additional Functionality

  * NFC Card Reader
  * Rotary Encoder
  * Per Key Addressable Backlighting

## Novelkey Novelty macropad
[![Novelkey Novelty Big Switch Macropad](/assets/images/novelkey.jpeg)](/novelkey-big-switch/README.md)

### Additional Functionality

  * Per Key LED Backlighting
  * BIG switches

# Hardware Used
  * 1 x ESP8266 / NodeMCU
  * 9 x Relegendable KeyCaps (waterslide decal paper can also be used with existing keycaps, especially blank ones)
  * 9 x Mechanical key switches
  * Hot Glue
  * 3d printer material
  * various wire

# STL Files for 3D Printing
All the case designs can be found on Github, [Printables](https://www.printables.com/@AeroSteveO/collections/1135401), and [Thingiverse](https://www.thingiverse.com/aerosteveo/collections/40893020/things)

# Configuration
EspHome YAML files are included with each project and are versioned to allow for legacy device support.

# Printing Instructions
These can be printed with low infill for speed and with a medium to thick layer height, they don't need a fine layer height to print well. All the designs are intended to be printed without supports (except the main enclosure for the novelkey novelty macropad). 

# Contributing
Contributions are welcome to the project

# Change Log

  * With generation 3, we begin to use the Matrix Keypad feature of EspHome, simplifying the wiring.
  * With generation 4, we'll be adding WS2812 LEDs to backlight the key switches, providing an aveneue for notifying of a status from home assistant
