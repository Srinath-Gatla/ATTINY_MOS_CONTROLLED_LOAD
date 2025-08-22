# ATTINY_MOS_CONTROLLED_LOAD
**Key Components**

U1 (ATtiny85)
Small 8-pin microcontroller providing logic control signals on its GPIO pins.

Q1, Q2, Q3 (IRLZ44N MOSFETs)
Logic-level N-channel MOSFETs, used as electronic switches to control current to the load.

Q1 and Q2 appear to be in a cascaded arrangement (one controlling the other).

Q3 looks like it is driving or enabling the stage.

R1, R3, R5 (220 Ω gate resistors)
Limit inrush current into the MOSFET gates when switching. This protects the ATtiny85 output pins and improves stability.

R2, R4, R6 (10 kΩ pull-down resistors)
Ensure that the MOSFET gates remain low (OFF) when the ATtiny85 pins are floating or during reset.

L1 (60 V lamp)
The load being driven.

V1 (50.4 V source)
The supply powering the circuit. 

Switch symbol (near R5)
A manual input switch to the ATtiny85 (probably simulating a push button).
