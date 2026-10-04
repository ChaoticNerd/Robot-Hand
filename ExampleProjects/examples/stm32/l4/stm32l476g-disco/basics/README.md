This demonstrates some basics on the L476G disco board.

* Blink green LED (PA5) on board
* No timer used, simple for loop stall
* GPIO & RCC are structs dictated in the stm32l476xx.h file
* stm32l476xx.h file and other headers are to be moved into /libopencm3-examples/libopencm3/include/libopencm3/stm32/l4
    * note: this folder contains headers for specific functions such as GPIO and TIMER; HOWEVER, they do not include the structs for them - I would personally continue using the stm32l476xx.h file
* Setup GPIO via RCC (specific bit)
* use GPIO MODER to set input vs. output for specific register
* use GPIO ODR to set output values for register
* simple timer usage.
