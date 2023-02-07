# Bidirectional_Visitor_Counter
PROBLEM STATEMENT: 

Design a credit card-sized counter device (images attached below for reference) that can keep a count on the occupancy of an indoor venue. The device is ideally mounted at the entrance of the room. The device has sensors to detect when a person enters or exits the room and can distinguish whether someone is ‘Entering’ or ‘Exiting’. The green and red circles indicated in the image below are indicative positions of the sensors. It has a 2-digit 7-segment display to show the count. As a guest enters the device detects and the count on the display increments by 1 with every guest entering. Similarly while exiting the guests the device detects and the count on the display decrements by 1. The simple solution helps inform guests about the occupancy and they can choose not to enter if the occupancy is near or above the spatial capacity of the venue. You’re tasked with designing the electronics for this device wherein you have to design a single 2-layered PCB that hosts all the electronic components needed. 





Working of the project:

The system is designed for optimum energy usage and is very beneficial in case if we want to count the number of people going to attend a particular event or any function thereby helps in collecting data by counting the number of people. This is done by simply incrementing the counter.
The system uses InfraRed Sensor pairs in order to fulfil this purpose and thus saves a large amount of energy. Each pair consists of 2 sensor pairs placed at a certain distance from one another in the opposite direction. The IR transmitter is used to transmit IR rays straight to the receiver which receives the input and feeds this to an 8051 Microcontroller.
As soon as a person enters the area where the system is placed, it is detected by the IR sensor module and this info is fed to the microcontroller. The microcontroller process this input received. At this time the system also counts the number of people present and increments a counter on each arrival, this count is displayed on a 7 segment display.
Summary




Microcontroller:

I have tried to design the PCB in Eagle Software. 
The main hardware I have used for the task is Arduino Nano. The reason behind using Nano is the that it has operating voltage of 5 V which is mentioned in the assignment. Apart from this the microcontroller which is Microchip ATmega328P is capable controller with flash memory if 32 KB which is more than sufficient for trivial tasks. 


Looking at the technical specifications of the Nano board, we find the following features:
 
o	ATmega328P Microcontroller is from the 8-bit AVR family
o	The operating voltage is 5V
o	Input voltage (Vin) is 7V to 12V
o	Input/Output Pins are 22
o	EEPROM is 1 KB
o	CLK speed is 16 MHz
o	Weight-7g
o	The size of the printed circuit board is 18 X 45mm
o	Supports three communications like SPI, IIC, & USART
o	Flash memory is 32 KB
o	SRAM is 2 KB
o	Analog i/p pins are 6 from A0 to A5
o	Digital pins are 14
o	Power consumption is 19 mA
o	I/O pins DC Current is 40 mA


IR Sensors

Tsop sensor: The tsop1738 is a infrared receiver tuned to react only to ir of frequency 38 khz. This ir sensor module consists of a pin diode and a pre amplifier which are embedded into a single package. The output of tsop is active low and it gives +5v in off state.


Display
7 segment display used is DS1 with 2 units of 74HC595 shift resisters for two wat 7 segment displays

Power Supply

The Arduino Uno can be powered via the USB connection or with an external power
supply. The power source is selected automatically. External (non-USB) power can come either
from an AC-to-DC adapter (wall-wart) or battery. The adapter can be connected by plugging a
2.1mm centre-positive plug into the board's power jack. Leads from a battery can be inserted in the
Gnd and Vin pin headers of the POWER connector.
The board can operate on an external supply of 6 to 20 volts. If supplied with less than 7V,
however, the 5V pin may supply less than five volts and the board may be unstable. If using more
than I2V, the voltage regulator may overheat and damage the board. The recommended range 1S /
to 12 volts
![image](https://user-images.githubusercontent.com/90505751/217337112-516ef2ec-346f-45bd-a955-2e303ff8cb41.png)
