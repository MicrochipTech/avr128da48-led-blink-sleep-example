# AVR128DA48 LED Blink with sleep and wake up using a Timer interrupt example

This repository provides an Atmel Studio solution with a bare metal code example for an LED blink and sleep application. The AVR-da is woken up from sleep using TCA0 interrupt. 

This example demonstrates simple toggling on a LED connected to PC6 with a period of 1 second. After toggling the LED, the device enters sleep until it gets woken up by an interrupt from TCA0.

## Configurations

* PC6 - configured as digital output (the on-board user LED)
* TCA0: 
	* Normal mode
	* Input clock Main Clock (4MHz) /256
	* Overflow interrupt enabled
	* Period 0x2000
* CPUINT:
	* Global interrupt enabled


## Required Tools 

Software: ATMEL Studio and AVR-DA Device Packs

Hardware: AVR128DA48 Curiosity Nano


## Compatibility
The source code is compatible with the following devices: AVR128DA28, AVR128DA32, AVR128DA48, AVR128DA64, ATmega4808, ATmega3208, ATmega1608, ATmega808, ATmega4809, ATmega3209, ATmega1609, ATmega809.




## AVR-DA LED blink with sleep and interrupt from timer wake-up

#### INTRODUCTION
This repository contains the project source code for the AVR128DA48 Curiosity Nano development board.

#### EXAMPLE DESCRIPTION

This example demonstrates simple toggling on a LED connected to PC6 with a period of 1 second. After toggling the LED, the device enters sleep until it gets woken up by an interrupt from TCA0.

#### RELATED DOCUMENTS / APPLICATION NOTES

Refer to Mcicrochip developer page for more details.

#### SUPPORTED EVALUATION KIT

AVR128DA48 Curiosity Nano development board.

#### INTERFACE SETTINGS

* Digital Output Pin: 
	* PC6 as LED0 pin 
* TCA0: 
	* Normal mode
	* Run in Standby enabled
	* Input clock Main Clock (4MHz) /256
	* Overflow interrupt enabled
	* Period 0x2000
* CPUINT:
	* Global interrupt enabled
* SLPCTRL
	* Standby mode

#### RUNNING THE DEMO

1. Select "EXPORT PROJECT" tab and click "Download Pack" to save the .atzip file.
2. Import .atzip file into Atmel Studio 7, File->Import->Atmel Start Project.
3. Build Solution and make sure no compiler error occur.
4. Press "Start without debugging" or use "CTRL+ALT+F5" hotkeys to run the application.

