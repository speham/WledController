# WledController

## Controller based on Esp8266-12F  for https://github.com/Aircoookie/WLED.git 

[![Shield](https://github.com/speham/WledController/ControllerClosed.jpg)](https://github.com/speham/WledController/ControllerClosed.jpg)

## Settings / Features
- SW Button - GPIO0  
- Data Pin  - GPIO2
- Serial Connection for flashing
- use fuse depending on maximum current of Led stripe (max 5A)
- OTA-Update possible
- small form factor (41x55x21mm)


## Compatible Led Stripes
WS2812B | 5v | RGB
SK6812  | 5v | RGBW

## Connections
Connect 5V/GND to power supply. 5V out should only be used for LED stripes with less than 60 Leds (3.6A - ws2812b)
For longer stripes only the data wire of the stripe should be connected to the controller so + and - of the LED stripe 
is connected to the power supply (common GND for controller and led stripe).


## Flash With Other Firmware
Serial connector on top right side of the board (FTDI adapter necessary to flash)
 - Hold boot and RST button
 - release RST button 
 -> brings the esp8266 in flash mode