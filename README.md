# arduino-game

## Instructions
Use a long hookup wire to connect the 5V signal on the Arduino to the far left of the red row at the top of the breadboard.

Use a long hookup wire to connect the GND signal to the far left of the black (or blue on some breadboards) row at the top of the breadboard.

The LCD (Liquid Crystal Display) module has a 16-pin male header on the underside. Plug this into the breadboard as shown in the picture. All of the electronic signals that power and control the LCD go through this header.

These pins are (from left to right):

GND - power ground signal
VCC - positive power signal
V0 - contrast adjust
RS - register select
R/W - read/write select
E - operation enable signal
DB0 - data bit 0 (not used here)
DB1 - data bit 1 (not used here)
DB2 - data bit 2 (not used here)
DB3 - data bit 3 (not used here)
DB4 - data bit 4
DB5 - data bit 5
DB6 - data bit 6
DB7 - data bit 7
LED+ - backlight LED positive
LED- - backlight LED negative
Using short hookup wires, connect GND and LED- (pins 1 and 16) to the black row at the top.

Similarly, connect VCC (pin 2) to the red row at the top with a short hookup wire.

Bend the wire leads of the 220 Ω resistor (red-red-brown colored bands) and connect it between LED+ and the red row at the top of the breadboard.

Use longer hookup wires to make the remainder of the connections:

Connect DB7 to Arduino pin 3
Connect DB6 to Arduino pin 4
Connect DB5 to Arduino pin 5
Connect DB4 to Arduino pin 6
Connect E to Arduino pin 9
Connect R/W to Arduino pin 10 (or to black row at top of breadboard)
Connect RS to Arduino pin 11
Connect V0 to Arduino pin 12 (or to black row at top of breadboard)
Plug the push button somewhere to the left of the LCD screen, straddling the channel running along the center of the breadboard (see picture above). Connect one of the top two pins of the button to the black row at the top of the breadboard using a short hookup wire. Connect the other pin at the top of the button to pin 2 of the Arduino.

## Reference

In this project, the code was based on Mohammed Magdy's "Arduino Game By LCD", but some of the basic behaviors (such as gravity) and the sprites images were changed to make the running man appear to be a flying bird.

url: https://create.arduino.cc/projecthub/muhamd-magdy/arduino-game-by-lcd-9a3bc2?ref=user&ref_id=8893&offset=0
