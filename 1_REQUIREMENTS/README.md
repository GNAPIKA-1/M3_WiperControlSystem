# COMPONENT
***STM32F407VG MICROCONTROLLER BOARD***
## Description
* The STM32F405xx and STM32F407xx family is based on the high-performance Arm® Cortex®-M4 32-bit RISC core operating at a frequency of up to 168 MHz.
*  The Cortex-M4 core features a Floating point unit (FPU) single precision which supports all Arm single-precision data-processing instructions and data types. 
*  It also implements a full set of DSP instructions and a memory protection unit (MPU) which enhances application security. 
*  The STM32F405xx and STM32F407xx family incorporates high-speed embedded system.


# WORKING PRINCIPLE
*The blinking of TM32F407VG Microcontroller LED's are considered as position of Wiper of an Automobile.If the push button is long pressed for 2sec , the first LED (red) will turn on. Where, the engine starts.Pressing the push button again, the LEDS,i.e;second led (blue) will turn on and off, the third led (green) will turn on and off,then,the fourth led (orange) will turn on and off, moving at a desired rate by blinking away the LED's.Later, clicking, next time the button, the blue, green and orange LEDs will blink fast at other frequency.Last,the microcontroller (vehicle) is turned off after the long press for 2sec.*

# 4W's & 1H
 **What**  : Automatic Wiper Control System using the microcontroller STM32F407VG .
 **When**  : When the visibility of the road is compromised due to rain, snow, dust.
 **Where** : On the windshield of the vehicle.
 **Why**   : To improve the visibility of the road, to prevent accidents and to ensure safe travel.
 **How**   : By designing an embedded system controller to control the wiper arm action according to severity of conditions without human intervention.
# SWOT ANALYSIS
## STRENGTH
* Less Cost.
* User friendly.
* Standardized.
* Mass production.
## WEAKNESS
* Sturctural mass.
* Huge transport cost.
* Not flexible.
## OPPORTUNITIES
* Emergence of new innovations.
* Industrial growth through lead in technology.
* Demand and Supply.
## THREATS
* not waterproof.
* not fireproof.
* No validity.
* Economical Crisis.




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
