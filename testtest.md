#Pressure Plate Puzzle

For the escape room, one of the puzzles involves a set of pressure plates. There are 8 pressure plates which can be set up in any configuration. The plates need to be pressed in a certain order at a certain tempo in order to complete the puzzle.

##Construction
The plates need to register two states: Unpressed and pressed. This is accomplished by an open circuit that is closed by contact with the plates. In addition, they need to be durable so people can step on them repeatedly. The last important criterion was that the plates should be able to register a step no matter which part of the plate is pressed. 
####Hardware
1\16 inch lexan sheets were used for the top and bottom of the pressure plates. Small pieces of neoprene were used around the edges to separate the plates. The neoprene is a slightly compressible material that is also electrically insulating. The resulting gap between the plates is very small, allowing room for the top lexan sheet to flex without breaking to make contact with the bottom plate. Because of the flexibility of the thin lexan, contact can be achieved no matter which part is pressed. 
The top plate is distinguishable from the bottom plate because of the rectanglular space free of aluminum foil in the middle. This is to prevent accidental contact where there is the most likely chance of it happening. The bottom plate is completely covered in aluminum foil to ensure contact wherever is pressed. 
####Circuits
Each pressure plate assembly creates its own individual circuit containing a high voltage rail, a ground rail, an LED, two resistors, and a connection to a digital pin of the Arduino Mega. A pull-down resistor connects the digital input pin to ground so it will always read a low voltage until the pressure plate is stepped on. When the aluminum foil on each plate makes contact, the circuit is completed and the pin is driven high. 
