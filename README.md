
---


## Description

PwRberry board is a power management HAT for raspberry PI to take care of proper power-on, power-off, wake-up, Reset, or power-cycle RPI using external control sources.

![](https://user-images.githubusercontent.com/58411599/123131621-251b0f00-d44e-11eb-9ba9-3fcc5851ea36.png)


To optimize the cost for specific application users can customize the board to their needs via connecting external breakouts for the following scenarios:

- **Power Button:** PwRberry allows the user to connect external switches to GPIO pins specially designed to connect to mechanical buttons with protection and denouncing implemented.


- **WiFi:** using ESP8266 / ESP32 wifi modules connected to PwRberry pins.

![](https://user-images.githubusercontent.com/58411599/123131606-22201e80-d44e-11eb-8fef-258fe750e7a5.png)
 
  
- **Bluetooth / BLE:** using nRF52 or any other BLE modules.

![breakouts-ble](https://user-images.githubusercontent.com/58411599/123131591-1df40100-d44e-11eb-8ea5-66804fe1872c.png)
  
  

- **Ethernet Wake-on-LAN (WoL):** connecting enc28j60 breakout board to PwRberry adds extra RJ-45 port make it possible  to bring raspberry PI out from power down state after receiving WoL magic packet.

![breakouts-eth](https://user-images.githubusercontent.com/58411599/123131597-1fbdc480-d44e-11eb-9542-eba984727c35.png)

- **HDMI-cec:** developer can connect HDMI connector breakout to PwRberry pins and configure it to respond to HDMI-cec bus commands.



![breakouts-hdmi](https://user-images.githubusercontent.com/58411599/123131599-20565b00-d44e-11eb-995e-36625f8c4348.png)  



- **IR remote:** PwRberry supports connecting an IR receiver and be controlled via TV remote-control power button 

![breakouts-ir](https://user-images.githubusercontent.com/58411599/123131605-21878800-d44e-11eb-8453-e4e9e5656e5a.png)

- **RTC:** PwRberry HAT implements internal real-time time-keeper RTC and can be scheduled to wake-up and shutdown RPI via simple script

- **Serial:** PwRberry has UART pins exposed for custom use. and It can used to connect transceivers like RS485 / RS422 / RS232 and can decode MODBUS packets. SPI and I2C is also supported.



**Raspberry PI power management is important for**: 

- **Saving connected peripherals life:** shutting down Raspberry PI via software will NOT cut the power from connected peripherals such as Flash / HDD drive, 4G/5G modem, etc. And for peripheral reliability and extended life it's safe to power down the connected peripheral when its not needed.

- **Robustness by periodic reboot:** although Raspberry PI can be left running for long periods while consuming negligible power, It's also important to periodically reboot the whole system for end application reliability

- **Remote power management:** In some IoT applications deployments as in agriculture, smart cities, industrial, etc. where you may not have physical access to the board to manually power-cycle  in case of software crash or malfunction

Also as raspberry PI 5V input power is NOT a standard voltage except for USB powered devices, PwRberry


HAT allows the developer to use Raspberry PI in wide application field deployments. By providing wide input voltage range for applications like : agriculture, automotive, marine, industrial-automation, home-automation, smart-cities, surveillance, computer vision, .. etc.



## Features

- input power :  36VDC ~ 6VDC
- Maximum current: up to 10A  
- RPI power control : power-SW , soft-GPIO [Raspberry PI header pins] 
- ports/pins: HDMI-cec, IR-receiver, Ethernet-WoL, UART, IoT-modules, RTC, Buttons
- Temperature range: 0 ~ +85C






