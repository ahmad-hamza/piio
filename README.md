
---


## Description

Raspower board is a power management HAT for raspberry PI to take care of proper power-on, power-off, wake-up, Reset, or power-cycle RPI using external control sources.



To optimize the cost for specific application users can customize the board to their needs via connecting external breakouts for the following scenarios:

- **Power Button:** Raspower allows the user to connect external switches to GPIO pins specially designed to connect to mechanical buttons with protection and denouncing implemented.
- **WiFi:** using ESP8266 / ESP32 wifi modules connected to Raspower pins.
- **Bluetooth / BLE:** using nRF52 or any other BLE modules.
- **Ethernet Wake-on-LAN (WoL):** connecting enc28j60 breakout board to Raspower adds extra RJ-45 port make it possible  to bring raspberry PI out from power down state after receiving WoL magic packet.

- **HDMI-cec:** developer can connect HDMI connector breakout to Raspower pins and configure it to respond to HDMI-cec bus commands.

- **IR remote:** Raspower supports connecting an IR receiver and be controlled via TV remote-control power button 

- **RTC:** Raspower HAT implements internal real-time time-keeper RTC and can be scheduled to wake-up and shutdown RPI via simple script

- **Serial:** Raspower has UART pins exposed for custom use. and It can used to connect transceivers like RS485 / RS422 / RS232 and can decode MODBUS packets. SPI and I2C is also supported.



**Raspberry PI power management is important for**: 

- **Saving connected peripherals life:** shutting down Raspberry PI via software will NOT cut the power from connected peripherals such as Flash / HDD drive, 4G/5G modem, etc. And for peripheral reliability and extended life it's safe to power down the connected peripheral when its not needed.

- **Robustness by periodic reboot:** although Raspberry PI can be left running for long periods while consuming negligible power, It's also important to periodically reboot the whole system for end application reliability

- **Remote power management:** In some IoT applications deployments as in agriculture, smart cities, industrial, etc. where you may not have physical access to the board to manually power-cycle  in case of software crash or malfunction

Also as raspberry PI 5V input power is NOT a standard voltage except for USB powered devices, Raspower HAT allows the developer to use Raspberry PI in wide application field deployments. By providing wide input voltage range for applications like : agriculture, automotive, marine, industrial-automation, home-automation, smart-cities, surveillance, computer vision, .. etc.



## Features

- input power :  24VDC ~ 6VDC
- Maximum current: up to 5A  
- RPI power control : power-SW , soft-GPIO [Raspberry PI header pins] 
- ports/pins: HDMI-cec, IR-receiver, Ethernet-WoL, UART, IoT-modules, RTC, Buttons
- Temperature range: 0 ~ +85C






