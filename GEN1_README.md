# Functionality
ESPDeck provides a macropad type input set to Home Assistant based on ESPHome. This includes 3 modes of input for each keyswitch. 

  * Single Click
  * Double Click
  * Click and Hold

# Hardware Used
  * 1 x ESP8266 / NodeMCU
  * 9 xRelegendable KeyCaps (waterslide decal paper can also be used with existing keycaps, especially blank ones)
  * 9 x Mechanical key switches
  * Hot Glue
  * 3d printer material
  * 9 x 10k Ohm Resistors

# Wiring
## Gen1 Design
3.3V to the switches

10k to ground for each Digitial IO Pin, as well as a line to the switch

![First Generation Circuit Diagram](/assets/images/circuit-gen1.svg)

# Configuration
keypad.yaml
