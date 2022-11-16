# IS62 SPI SRAM Pi Pico SRAM Micropython and C/C++ SDK Driver

Here you'll find the datasheet and the Micropython and C/C++ drivers for the IS62 SPI SRAM module from ISSI.
The Micropython driver is fairly rudimentary but it should serve as a good way to get started with interfacing with the SRAM- my first
attempt with anything Pi Pico related so... yeah. 

Note that the circuit diagram is old: I will update this in due time with a new example component list/etc. 

## Circuit.png 
Example circuit diagram. Decoupling caps are included including a ferrite to isolate from the 3V3 noise on the Pico.

## IS62_DRIVER.py 
Micropython (basically pseudo)-code. Works well enough- copy from the C code if you need more.

## c_drivers
C code. Uses the SDK. Has some ADC DMA example code in it (this is for a bat recorder project after all.) Includes quality-of-life
functions for reading/writing 16-bit data to the SRAM for the sake of recording from the ADC. Now includes a header file, too. 