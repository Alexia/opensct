#Integrated Circuits
##ARM Cortex-M4 ST STM32F427
* Crypto
* 2x CAN bus controllers
* Most likely used for CAN bus interface.
* JTAG Pins - Left to right
	* VSS_1/2/3(Pin 27/74/99) - JTAG Pin 1
	* VDD_1/2/3(Pins 50/75/100) - JTAG Pin 2
	* NRST(Pin 14) - JTAG Pin 3
	* NJTRST - PB4(Pin 90) - JTAG Pin 4
	* JTDO - PB3(Pin 89) - JTAG Pin 5
	* JTDI - PA15(Pin 77) - JTAG Pin 6
	* NC - JTAG Pin 7
	* JTCK - PA14(Pin 76) - JTAG Pin 8
	* JTMS - PA13(Pin 72) - JTAG Pin 9

##ARM Cortex-M3 ST STM32F103RB (64-pin)
* 128kb Flash
* USB
* CAN

##ARM Cortex-M3 ST STM32F103VE (100-pin)
* 512kb Flash
* USB
* CAN
* Most likely used for custom USB interface.
* JTAG Pins - Left to right from Micro USB connector
	* VSS_1/2/3(Pin 49/74/99) - JTAG Pin 1
	* VDD_1/2/3(Pins 50/75/100) - JTAG Pin 2
	* NRST(Pin 14) - JTAG Pin 3
	* NJTRST - PB4(Pin 90) - JTAG Pin 4
	* JTDO - PB3(Pin 89) - JTAG Pin 5
	* JTDI - PA15(Pin 77) - JTAG Pin 6
	* NC - JTAG Pin 7
	* JTCK - PA14(Pin 76) - JTAG Pin 8
	* JTMS - PA13(Pin 72) - JTAG Pin 9
* Micro Switch
	* Pulls PB0(Pin 35) to ground - Default: ADC12_IN8/TIM3_CH3/TIM8_CH2N, Remap: TIM1_CH2N

##Texas Instruments CC3000MOD
* 802.11b/g Wireless Radio

#Other Bits
* Coin Cell Battery for Real Time Clock
* 4gb Micro SD Card, FAT16 Formatted