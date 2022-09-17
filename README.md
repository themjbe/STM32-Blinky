# STM32-Blinky

Course Making Embedded Systems
Cohort 3
Activity ID mes3_l4_ex_make-blinky

This is an example of using STM32CubeIDE to create a blinky application for the STM32F411E-DISCO board.

There are four LEDs on the board.

Green and Orange alternate increasing and decreasing brightness

Blue - lit when orange is increasing and green is decreasing
Red - lit when orange is decreasing and green is increasing


What are the hardware registers that cause the LED to turn on and off? (From the
processor manual, don’t worry about initialization.)

STM32CubeIDE allowed me to define these in the ioc file as BLED (PD15), RLED (PD14), OLED (PD13), and GLED (PD12)
GPIOD_ODR is the register used by the HAL

● What are the registers that you read in order to find out the state of the button?

GPIO input labeled B1 (PA0), used HAL so didn't need to know specific registers
GPIOA_IDR is the register used by the HAL

● Can you read the register directly and see the button change in a debugger or by
printing out these value of the memory at the register’s address?

The ST-LINK and STMCubeIDE made this very easy