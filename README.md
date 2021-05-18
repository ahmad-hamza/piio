---
## Introduction

PwRHAT is a power management HAT for raspberry PI to take care of proper wake-up, Reset, shutdown, or power-cycle RPI using input from Ethernet-WoL, HDMI-cec, IR-remote, Serial(UART/SPI), RS485/rs422/RS232, modbus, WiFi, Bluetooth/BLE. 
As power management is important for: 

- **Saving connected peripherals life:** shutting down Raspberry PI via software will NOT cut the power from connected peripherals such as flash/HDD drive, 4G/5G modem, etc. And for peripheral reliability and extended life it's safe to power down the connected peripheral when its not needed.

- **Robustness by periodic reboot:** although Raspberry PI can be left running for long periods while consuming negligible power, It's also important to periodically reboot the whole system for end application reliability

- **Remote power management:** In some IoT applications deployments as in agriculture, smart cities, industrial, etc. where you may not have physical access to the board to manually power-cycle  in case of software crash or malfunction

Also as raspberry PI 5V input power is NOT a standard voltage except for USB powered devices, PwRHAT allows the developer to use Raspberry PI in wide application field deployments. By providing wide input voltage range for applications like : agriculture, automotive, marine, industrial-automation, home-automation, smart-cities, surveillance, computer vision, .. etc.



## Features

- input power :  60VDC ~ 6VDC
- Maximum current: up to 8A 
- RPI power control : power-SW , soft-GPIO [Raspberry PI header pins] 
- ports/pins: HDMI-cec, IR-reciever, Ethernet-WoL, UART, IoT-modules, RTC, Buttons
- Temperture range: 0 ~ +85C



## Description

PwRHAT controls raspberry PI power via a switch connected between the regulator and RPI 5V power input at the GPIO header pins. it also can initiate soft shutdown / wake-up / reset via RPI GPIO pins.

To optimize the cost for specific needs so the users can customize the board to his needs, PwRHAT is compatible with Breakout boards for the following scenarios:


- **Ethernet Wake-on-LAN (WoL):** connecting enc60j28 breakout board to PwRHAT adds extra RJ45 port make it possible  to bring raspberry PI out from power down state after receiving WoL magic packet 

	

- **HDMI-cec:** developer can connect HDMI connector breakout to PwRHAT pins and configure it to respond to HDMI-cec bus commands.

- **IR remote:** developer can connect IR receiver to PwRHAT and program the remote-control power button 

- **RTC:** PwRHAT implements internal real-time time-keeper RTC and can be scheduled to wake-up and shutdown RPI via simple script

- **UART:** PwRHAT has UART pins exposed for custom use. and It can used to connect transivers like RS485/rs422/RS232 and can decode MODBUS packets 

- **GPIO:** In addition to general-perpose input pins specially designed to connect to mechanical buttons with protection and denouncing implemented 

- **IoT:** PwRHAT also accepts IoT modules for WIFI, bluetooth/BLE.


