# Debug using Segger Ozone

Segger Ozone is one of the most used visual debuggers used for debugging ARM Cortex-M controllers. This guide will help you get started.

## Prerequisites
To be able to debug using Segger Ozone you need the following:
- Segger Ozone installed on your pc
- The ST-Link probe on the F0DiscoveryProbe needs to be flashed with the JLink firmware

### Installing Segger Ozone
> See [installation.md](installation.md) for the installation instructions

### Flashing the JLink firmware to the F0DiscoveryProbe
> See the [Segger guide](https://www.segger.com/products/debug-probes/j-link/models/other-j-links/st-link-on-board/) for the instructions on how to flash the firmware.

> Scroll down to the `Getting Started with ST-LINK On-Board` section and follow the steps.

## Getting started

First read the [official Segger Ozone guide](https://www.segger.com/products/development-tools/ozone-j-link-debugger/technology/getting-started-with-ozone/) before proceeding. 

## New project wizard
Open the New Project wizard. 

**These options are very important, all the other options can be left at default:**

### Device: Select the right device
The device to select is the STM32F050C6. This will load the correct device options in to segger Ozone.

### Peripherals: Use the .svd file provided in the bsp folder of this repo
When using the New Project wizard select the .svd file in the `Peripherals (optional)` option.

The .svd file describes the hardware peripheral registers and provides the memory locations. When Segger Ozone is configured to use this file it allows you to see straight in to the hardware peripheral registers of the device.

### Data File (optional): Select the executable

Select the *.elf executable from the build directory.
