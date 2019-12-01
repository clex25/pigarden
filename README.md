# pigarden
_Inspired by Reef-Pi_

Home garden automation - measure the pH, temperature, humidity, atmospheric pressure, EC, soil temperature, soil moisture, light, and plant height using a custom sensor interface board which connects to raspberry pi GPIOs, and display/monitor it using a fancy web interface.

####Sensors:
* Atlas scientific EZO pH
* Atlas scientific EZO EC
* atlas scientific EZO isolation boards (x2 - voltage isolation for ph and ec)
* DS18B20 one wire digital temperature probe
* spark fun soil moisture 
* RHT03 humidity 
* HC-SR04 ultrasonic distance 
* T5403 barometric pressure 
* TSL2561 luminosity

**/hardware/** contains KiCad schematics and footprint files for the custom PCB which handles interfacing with all the sensors using

pigarden.py is the main python file which provides the interface between the pi and the sensors using I2C, serial, and digital I/O. 

Ultimately, I aim to fork ReefPi to add more supported sensors, and use the web interface and data collection from that project. 

This is still an early work in progress.