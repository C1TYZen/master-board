# master-board
Hardware and Firmware of the Solo Quadruped Master Board. 

This board centralises all the sensor and actuator data and provides wired and wireless connection to a realtime computer.

Connectivity:

* SPI: Address up to 8 SPI Slave: (max 80Mhz, DMA capable) compatible with BLMC µDriver SPI interface
* Wifi: Wireless communication with a computer via raw ESP-NOW: round trip time of 1.2ms (including driver and OS latency) for a 127bytes message.
* Ethernet: Wired communication with a computer via raw frames: round trip time of 0.2ms (including driver and OS latency) for a 127bytes message.
* GPIO: 4GPIO free. Can be mapped to I2C, UART etc.. Two of them are curently used for IMU communication via UART
* UART: Used to upgrade the ESP32 firmware, free on normal operation.

The board is programed via the ESP-IDF tool chain https://github.com/espressif/esp-idf

Wireless closed loop control at 1kHz demo (click to see video):
[![Alt text](https://img.youtube.com/vi/P_yazdwLeZ8/0.jpg)](https://www.youtube.com/watch?v=P_yazdwLeZ8)

IMU, ethernet closed loop cntrol at 1kHz demo (click to see video):
[![Alt text](https://img.youtube.com/vi/-jNc_tuRp-E/0.jpg)](https://www.youtube.com/watch?v=-jNc_tuRp-E)

Authors
--------
Thomas Flayols  
Etienne Arlaud

License
-------
BSD 3-Clause License

Copyright
-----------
Copyright (c) 2019, LAAS-CNRS, Max Planck Gesellschaft, New York University

More Information
----------------
[Open Dynamic Robot Initiative](https://open-dynamic-robot-initiative.github.io)  
