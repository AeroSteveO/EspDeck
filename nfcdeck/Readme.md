# NFC Deck
This is a complex iteration of the EspDeck in order to allow control of multi room audio systems (or anything else you want to use it for). There are two top panel iterations, one for 9 mechanical key switches, and one for 8 key switches and one rotary encoder.

# Components:
  * ESP32 DevKitv1
  * 8  x Mechanical Key Switches
  * 1  x Rotary Encoder
  * 1  x NFC Card Reader
  * 10 x WS2812 LEDs
  * 1  x Piezo Buzzer
  * 4 x [Rubber Feet](https://www.amazon.com/dp/B06XPCLN23)

# Circuit Diagram
![First Generation Circuit Diagram](/nfcdeck/assets/nfcdeck_circuit.svg)

# Wiring

# Assembly

- Print out the top plate, and mount all of your key switches to it and the rotary encoder.
- Solder all the key switches and rotary up to the D1 Mini


Also, make sure that you have set the switches on the PN532 to the following:
- Switch 1: On (up)
- Switch 2: Off (down)

This enables the PN532 module to communicate with the D1 over I2C, and is required for the modules to work together!

# Printing Instructions
Print one each of:

 *  nfcdeck_base.stl
 *  NfcDeck Top Piece (one of either option)
	*  nfcdeck_top_rotary.stl (with a space for a rotary encoder)
	*  nfcdeck_top_9key.stl (with 9 key switches and no rotary encoder)

These can be low infill as they don't require much structural stability
