# EspDeck


ESPHome Based StreamDeck Type Macro Pad

# Functionality
ESPDeck provides a macropad type input set to Home Assistant based on ESPHome. This includes 3 modes of input for each keyswitch. 

  * Single Click
  * Double Click
  * Click and Hold

# Case

Case design based off of: https://www.thingiverse.com/thing:5204033. I extended the height of the case for my inefficient use of space inside of it, I also made some modifications to better hold the Esp8266

Case design can also be found here: https://www.thingiverse.com/thing:5223223


# Wiring
# Gen1 Design
![First Generation Circuit Diagram](/assets/images/circuit-gen1.svg)

## Gen2 Design
![Second Generation Circuit Diagram](/assets/images/circuit-gen2-full.svg)


![Second Generation Circuit Diagram Simplified](/assets/images/circuit-gen2-simplified.svg)

## Gen1
3.3V to the switches

10k to ground for each Digitial IO Pin, as well as a line to the switch

## Gen2
Since it seemed like the resistors weren't needed, the wiring can be simplified to one end of the switch going to the digitial IO pin, and the other end to ground, and set up ESPHome to have the internal pullup enabled on the ESP8266 device.

# Contributing
Contributions are welcome to the project

