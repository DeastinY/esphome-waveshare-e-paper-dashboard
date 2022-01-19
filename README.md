# ESPHome Dashboard
Dashboard for office Co2 and some plant swag

![](https://github.com/DeastinY/esphome-waveshare-e-paper-dashboard/blob/main/dash.jpg?raw=true)

Inspired by: https://github.com/maxmacstn/HA-ePaper-Display  
Thanks for the nice repository!

## Hardware:
1. Waveshare 4.2" ePaper module
2. ESP32 NODEMCU

## Case
I did not find anything fitting yet, so currently attempting my own design.

## Information
With the dashboard sitting on my desk it most prominently displays Co2 ppm from a Netatmo weatherstation to remind me to open the windows.  
It also shows temperature and humidity from the same station. In addition stats from a VegTrug Soil Tester is shown on the bottom half.
 
### Wiring: 

|Waveshare| ESP32 Pin|
|--|--|
| BUSY | GPIO27 |
| RST | GPIO33  |
| DC | GPIO25 |
| CS | GPIO26 |
| CLK | GPIO18 |
| MOSI | GPIO23 |
| GND | GND |
| 3.3v | 3.3v |


## How to use?

 1. Install ESPhome on your [computer](https://esphome.io/guides/getting_started_command_line.html) or [Home Assistant Add-on](https://esphome.io/guides/getting_started_hassio.html)
 2. Copy yaml file and fonts folder to your ESPhome folder.
 3. Edit your Wi-Fi SSID/Password, sensors entity ID, etc. as your own preference.
 4. Connect hardwares together.
 5. Flash the firmware.
 6. Go to Home Assistant, it should automatically discovered your espHome display. If not, add it manually using IP address via ESPhome integration.
 7. Enjoy!
