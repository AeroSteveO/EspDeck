# NFC Deck
This is a complex iteration of the EspDeck in order to allow control of multi room audio systems (or anything else you want to use it for). There are two top panel iterations, one for 9 mechanical key switches, and one for 8 key switches and one rotary encoder.

# Variants:
  * 8 Keys, 1 Rotary Knob
  * 9 Keys
  * 2 Keys, 1 Rotary Knob
  * 3 Keys

# Components:
Since this has a few different variants you can build. We split the parts list up into the common parts for all models, and then the parts specific to each model. This are mostly different based on the counts for different parts.

## Common to All
  * ESP32 DevKitv1
  * 1 x NFC Card Reader
  * 1 x Piezo Buzzer
  * 4 x [Rubber Feet](https://www.amazon.com/dp/B06XPCLN23)

## 9 Key + Rotary
  * 8  x Mechanical Key Switches
  * 8  x Relegendable Key Caps
  * 1  x Rotary Encoder
  * 1  x Knob
  * 8  x WS2812 LEDs
  * 2  x 100 ohm resistors
  * 2  x 1 uf capcitors

## 9 Key
  * 9  x Mechanical Key Switches
  * 9  x Relegendable Key Caps
  * 9 x WS2812 LEDs

## 3 Key + Rotary
  * 2  x Mechanical Key Switches
  * 2  x Relegendable Key Caps
  * 1  x Rotary Encoder
  * 1  x Knob
  * 2  x WS2812 LEDs
  * 2  x 100 ohm resistors
  * 2  x 1 uf capcitors

## 3 Key
  * 3  x Mechanical Key Switches
  * 3  x Relegendable Key Caps
  * 3 x WS2812 LEDs

# Circuit Diagram
![First Generation Circuit Diagram](/nfcdeck/assets/nfcdeck_circuit.svg)

# Wiring
- Assemble a small circuit board with the rotary encoder 

# Assembly

- Print out the top plate, and mount all of your key switches to it and the rotary encoder.
- Solder all the key switches and rotary up to the D1 Mini

Also, make sure that you have set the switches on the PN532 to the following:
- Switch 1: On (up)
- Switch 2: Off (down)

This enables the PN532 module to communicate with the D1 over I2C, and is required for the modules to work together!

- Optionally electrical tape over the NFC module power LED

Mount the NFC module to the top plate


# Printing Instructions
Print one each of:

 *  nfcdeck_base.stl
 *  NfcDeck Top Piece (one of either option)
	*  nfcdeck_top_rotary.stl (with a space for a rotary encoder)
	*  nfcdeck_top_9key.stl   (with 9 key switches and no rotary encoder)

These can be low infill as they don't require much structural stability
Do use a slightly larger layer thickness for the top piece, 0.15mm is good, or more. The details come out a bit better in the home assistant logo using that higher layer thickness.

Work is still continuing on the 3 key designs, so they aren't yet available.