# bobble-nrf52
Bobble for Bluefruit nRF52832 has been created by derrick @ reachandteach.com and is a modified  version of sample code for Adafruit's nRF52 bleuart sample code.
 
The intent of this software is to create a simple preprogrammed controller to experiment with an attached motor or servo for controlling toys or other applications. 
 
Adafruit developed code has been provided under an MIT license, check LICENSE for more information

Any additional code by Reach and Teach is provided under a Creative Commons license allowing free use as long as attribution and share-alike licensing is respected.

The software accepts and responds to single character inputs:

'+' Sets MOTORENABLE (pin 7) HIGH 

'-' Sets MOTORENABLE (pin 7) LOW

 '0' - '9' Drives pin 11 as a PWM servo output from 0 degrees to 180 degrees in 20 degree increments
 
 'F' Sets MOTOROUT1 (pin 16) HIGH and MOTOROUT2 (pin 15) LOW
 
 'R' Sets MOTOROUT2 (pin 16) LOW and MOTOROUT2 (pin 15) HIGH
 
 'x' Reads an attached sensor voltage on A0
 
 '>' Sets high trigger value to last sensor reading
 
 '<' Sets low trigger value to last sensor reading
 
 '^' Sets low and high trigger for digital threshold
 
 ')' Sets command triggered by high trigger value to last command
 
 '(' Sets command triggered by low trigger value to last command
 
 '!' Enable sensor triggering

 '.' Disable sensor triggering
 
Pins 7, 16, and 15 are designed to be connected to a L293DNE motor driver chip to drive a toy motor. Pin 7 will be connected to the EN chip enable pin. Pin 16 and Pin 15 will be connected to the A chip pins. The motor will be connected to the Y chip pins.

MOTORENABLE (pin 7) can also be used to control an external AC/DC Relay Outlet like an Adafruit Controllable Four Outlet Power Relay Module version 2

A companion App Inventor 2 application has been written to allow an Android to easily communicate with this application. Contact derrick@reachandteach.com for more info.

