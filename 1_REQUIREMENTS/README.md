
# COMPONENT
***STM32F407VG MICROCONTROLLER BOARD***
## Description
* The STM32F405xx and STM32F407xx family is based on the high-performance Arm® Cortex®-M4 32-bit RISC core operating at a frequency of up to 168 MHz.
*  The Cortex-M4 core features a Floating point unit (FPU) single precision which supports all Arm single-precision data-processing instructions and data types. 
*  It also implements a full set of DSP instructions and a memory protection unit (MPU) which enhances application security. 
*  The STM32F405xx and STM32F407xx family incorporates high-speed embedded system.

# SOFTWARE REQUIREMENTS

### STM32 IDE:
* STMicroelectronics' STM32 family of 32-bit ARM Cortex-M core-based microcontrollers is supported by a wide range of software integrated development environments (IDEs).
### QEMU:
* Qemu is a machine emulator that can run operating systems and programs for one machine on a different machine.

## Xpack Packages :

### Windows Build Tools
* The xPack Windows Build Tools is a standalone Windows binary distribution of GNU make and a few of other tools required by the Eclipse Embedded CDT (formerly GNU MCU/ARM Eclipse) project, but the binaries can also be used in generic build environments.
### OpenOCD 
* Open On-Chip Debugger (OpenOCD) is a free, open-source project that aims to provide debugging, in-system programming, and boundary scan using a debug adapter. 
* The adapter is a hardware module that provides the right signals for the target to understand.


### QEMU 
* The xPack QEMU Arm is a standalone cross-platform binary distribution of QEMU, with several extensions for Arm Cortex-M devices.


# FEATURES OF STM32F407VG MICROCONTROLLER
* Memories
>Up to 1 Mbyte of Flash memory.
>Up to 192+4 Kbytes of SRAM including 64-Kbyte of CCM (core coupled memory) data RAM.
>512 bytes of OTP memory.
>Flexible static memory controller supporting Compact Flash, SRAM, PSRAM, NOR and NAND memories. 

* Clock, reset and supply management
>1.8 V to 3.6 V application supply and I/Os
>POR, PDR, PVD and BOR
>4-to-26 MHz crystal oscillator
>Internal 16 MHz factory-trimmed RC (1% accuracy)
>32 kHz oscillator for RTC with calibration
>Internal 32 kHz RC with calibration
* Low-power operation
* 3×12-bit, 2.4 MSPS A/D converters: up to 24 channels
* 2×12-bit D/A converters
* Upto 17 timers,etc

# WORKING PRINCIPLE
* Assume that the automobile is the microcontroller. 
* If the push button is long pressed , the first led (red) will turn on. Hence, the engine starts.
* Clicking the push button again, the wiper will start, and the second led (blue) will turn on, moving at a desired rate. 
* If the button is clicked again, the third led (green) will turn on, and the wiper's speed will be increased in comparison to the previous one. 
* With the fourth press,  the fourth led (orange) will turn on, and the wiper speed will be increased in accordance with the previous one. 
* The microcontroller (vehicle) is turned off after the fifth press which would a long press.


# SWOT ANALYSIS
## STRENGTH
* Low Budget
* Easy usage
* Good Reputation
* Big Influence on the market
## WEAKNESS
* Structural Inertia
* High Transaction Cost
* Weak Focus on Process Innovations
## OPPORTUNITIES
* Emerging New Markets
* Technological Development
* Demand for Saving Equipments
## THREATS
* Low Bargaining Power Buyers
* Ethical Pressure
* Highly Regulated Industry
* Economical Crisis
# 4W's & 1H
### WHAT
* The operational speed of a vehicle wiper is controlled by a wiper speed control mechanism based on rain conditions. To generate, the control system incorporates a rain sensor that detects rain conditions. The amplitude of an analogue signal depends on the detected rain conditions.
### WHY
* To keep the windscreen clean enough to give adequate view at all times. 
### WHEN
* The windshield wipers remove rain and snow from the windshield, while the headlights improve visibility at night.
### WHO
* A wiper speed control system for an automobile manages the wiper's functioning speed in response to weather conditions which is helpful for the drivers.
### HOW
* You can adjust the speed of the car wiper system according to the rainfall.
### WHERE
* In general, car wipers are controlled by the stalk on the right side of the steering wheel.


# HIGH LEVEL REQUIREMENTS
|ID|DESCRIPTION|STATUS|
|:--|:----------|:-----|
|HLRQ1|Car wiper using STM32F407VG|IMPLEMENTED|
|HLRQ2|Led glowing in sequence|IMPLEMENTED|
|HLRQ3|Car on and off|IMPLEMENTED|
|HLRQ4|Wiper on and off|IMPLEMENTED|

# LOW LEVEL REQUIREMENTS
|ID|DESCRIPTION|STATUS|
|:--|:----------|:-----|
|LLRQ1|Push Button|IMPLEMENTED|
|LLRQ2|Red,Green,Blue,Orange Leds|IMPLEMENTED| 
