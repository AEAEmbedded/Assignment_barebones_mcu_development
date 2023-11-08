# Assignment_barebones_mcu_development

Hi! Cool to have you here :) This is a follow-up assignment to the Intro to CMake you had in the previous semester. Here you will learn to set-up your own development environment using nothing but the (CMSIS-)bsp[^1], hal library[^2], CMake, segger tools and the arm-gcc compiler. Because we want to see your creative skills we decided to not deliver any code. You have to create a fun little project using the hardware (and software skills) you have at the moment.

[^1]: Board Support Package (BSP) is a collection of software components that allows an operating system to function on a particular hardware platform. It includes low-level drivers, startup code, and other necessary files like linker scripts that initialize the hardware and provide mechanisms for the OS to interface with it. Specifically, for ARM Cortex-M0 based microcontrollers, the BSP might contain standardized CMSIS headers along with manufacturer-specific initialization code and headers, facilitating software development and system control.
[^2]: A HAL, or Hardware Abstraction Layer. Is a library (most of the time provided by the MCU manufacturer) that provides a simpler interface to control and communicate with the hardware components of a microcontroller.


## Hardware choice
You can choose between a STM32F0 discovery kit or FRDM-KL25Z. 

The STM32F0 discovery devkit is pretty barebones and doesn't have much hardware onboard.Just for fun an lcd and potentiometer is provided, you are not obliged to do anything with these accesoires though you can. You may also choose to combine the devkit with a Roomba and do fun stuff using the SCI port.

The FRDM-KL25Z is a devkit most of you are probably familair with from the MIC2 course. It is a fun little devkit with a RGB led and accelerometer onboard. Of course you may choose to add a display or any other accesoire to this option. Do whatever suits you.
 
## Software preparation
For this assignment you need the following software installed:
- arm-none-eabi-gcc toolchain (Supplied with the Raspberry Pi Pico SDK)
- CMake (Supplied with the Raspberry Pi Pico SDK)
- Segger tools (Installed in the intro to CMake workshop)
- Segger Ozone (You need to install this, as it is the first time you might use this!)
- Any code editor you would like to use, vscode and clion presets are supplied in this repo.

For installation take a look at [installation.md](docs/installation.md)
