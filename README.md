#OneWire interface
The One-Wire interface is a communication protocol developed by Dallas Semiconductor, now part of Maxim Integrated, enabling devices to communicate using only a single wire for both data and power transmission. This protocol is particularly advantageous in scenarios where minimizing the number of wires is essential, such as in applications where running multiple wires is impractical.the Key Characteristics of the One-Wire Interface:
Single-Wire Implementation:
The One-Wire interface utilizes a solitary wire for both data and power transmission, simplifying wiring and reducing the number of required connectors.
Combined Data and Power Line:
Data and power are transmitted over the same wire. This is achieved through parasitic power, allowing connected devices to draw power from the data line during specific intervals.
Distinct Device Addressing:
Each device on the One-Wire bus is assigned a unique 64-bit address. This enables multiple devices to coexist on the same bus, with the master device addressing and communicating with individual devices based on their unique identifiers.
Variable Data Transfer Speeds:
The One-Wire protocol supports different data transfer speeds, ranging from standard speed (15.4 kbit/s) to overdrive speed (125 kbit/s).
Master-Slave Architecture:
Typically, the One-Wire bus operates in a master-slave architecture, where a master device initiates and controls communication with one or more slave devices.
Cost-Effective Implementation:
Due to its simplicity and the use of a single wire, the One-Wire interface is often considered a cost-effective solution for specific applications.
Applications:
Commonly used in various applications, the One-Wire interface finds usage in temperature sensors (e.g., DS18B20), real-time clocks, EEPROM memory, and other small embedded devices.
Reliability:
The One-Wire protocol is designed for reliability and robustness, making it suitable for deployment in challenging environments. 
Datasheets can be found in the Datasheets folder.
The goal of this project is to get a 1-wire device working and become familiar with the hardware and protocol. I included OneWire.h and OneWire.c in the project. For the temperature sensors I needed DS18x20.h and DS18x20.c in the project. to get started, I used the OWMain.c file provided and added LCD.h and LCD.c to the project.  All devices used RJ0 (PORTJ pin 0) as the DQ line. I needed a 4.7K – 5.1K pull-up resistor from DQ to 3.3V.


Requires:  
* Explorer 18 Board
* Pickit 3
* PIC18F87J11 Plugin module (PIM)
* One of the OneWire temperature sensors and/or EEPROM  

C programming Language.
