# ABSTRACT
## Project Name:
***Wiper Control System***
## Objective:
In this project, a high-performance **Arm® Cortex®-M4 32-bit RISC core**, STM32F407VG Microcontroller Board is used to demonstrate the working of ***Wiper Control System*** of an automobile at different states of modes and positioning the Wiper.
## Brief Explanation of Project:
>![illustration](https://user-images.githubusercontent.com/94955036/168634920-deb273a9-1d9f-4ab3-9c79-b9e6bf49c969.png)
>Automobiles have a unique design **ignition switch system**. The switch controls all the necessary components in the vehicle.The traditional vehicles with standard ignition system have four key positions. But modern vehicles have only three key positions.There is a specific action for every time you turn on the ignition switch.The ignition switch is the major part of an automobile and it is very important to keep this switch in the right shape.
>The second position switch is the **ACC/ACCESSORY position, which allows you to use your radio, windshield wipers**, and other accessories while the engine is off. This position should also be used in the event that your vehicle is being pushed or towed. In this position, the engine is off.(The next one is the ignition position. All the electronic accessories come active when you turn on the ignition switch in this mode. According to the expert maintenance tips, the ***ON position*** is the default position in vehicles.)
### Working:
In this project, we are enhancing the speed and frequency rate of Wiper and ensuring it in the correct position, so that Driver, catches the view of sight perfectly.Here, the LEDs of STM32F407VG Microcontroller are considered as Position of Wiper.Blue, Green and Orange are the LEDs.Alternately, the rate of frequency is taken from ON and OFF process to set frequency.When the PUSH Button is clicked Red LED will be ON.
#### Scenario:
- ***Ignition Key Position at ACC***: The Red LED is ON, if the user button is pressed and held for 2 secs
- ***Wiper ON: Wiper is OFF***: On press of the user input, Blue, Green and Orange LEDs come ON one at a time with the set frequency, The frequency changes on every alternate key press, 3 frequency levels with 1, 4 and 8 Hz
- ***Wiper OFF: Wiper is ON:*** The LED glow pattern stops on the 4th press; the wiper action starts next press onwards as mentioned in step 2
- ***Ignition Key Position at Lock***: The Red LED is OFF, if the user button is pressed and held for 2 secs
#### Different States of Mode:
| MODES  | CONDITION |
| ------------- | ------------- |
| MODE 1  |  Red LED is ON |
| MODE 2  |  Blue, Green and Orange LEDs ON at 1Hz  |
| MODE 3  |  Blue, Green and Orange LEDs ON at 4Hz   |
| MODE 4  |  Blue, Green and Orange LEDs ON at 8Hz   |
| MODE 5  |  Red LED is OFF |

Therefore, in this way, by considering different conditions,speed and frequency set, we need to complile a code that runs Wiper(LEDs) by an user interference and must positioned at initiatial state at the end.
## Structure:
### COMPONENT
***STM32F407VG MICROCONTROLLER BOARD***
![This is an image](https://robu.in/wp-content/uploads/2018/07/STM32F407-Discovery-Kit-for-STM32F407Robu-2.jpg)
>The STM32F405xx and STM32F407xx family is based on the high-performance Arm® Cortex®-M4 32-bit RISC core operating at a frequency of up to 168 MHz.
The Cortex-M4 core features a Floating point unit (FPU) single precision which supports all Arm single-precision data-processing instructions and data types. 
It also implements a full set of DSP instructions and a memory protection unit (MPU) which enhances application security. 
The STM32F405xx and STM32F407xx family incorporates high-speed embedded system.

## Software Used:
**STM32 IDE** -STMicroelectronics' STM32 family of 32-bit ARM Cortex-M core-based microcontrollers is supported by a wide range of software integrated development environments (IDEs) with C, C++, Pascal and JAVA support and debuggers from STMicroelectronics, allowing to configure and initialize the MCU or monitor its behavior in run time.

**QEMU** -It emulates the machine's processor through dynamic binary translation and provides a set of different hardware and device models for the machine, enabling it to run a variety of guest operating systems.
# WORKING PRINCIPLE
![work](https://user-images.githubusercontent.com/94955036/168655361-950b9164-23a7-47c9-939b-50ecc89e0a71.png)

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
# DESIGNS
The following are designs shown and classified below as follows;
# BLOCK DIAGRAM
![BLOCK DIAGRAM](https://user-images.githubusercontent.com/94955036/168512298-81fc8a9d-74ba-424b-9510-a5de305e2701.png)
# CLASS DIAGRAM
![CLASS DIAGRAM](https://user-images.githubusercontent.com/94955036/168512307-e601b82c-cd6d-4c73-a82a-21c2eb01a6f1.png)
# DATA FLOW DIAGRAM
![DATA FLOW DIAGRAM](https://user-images.githubusercontent.com/94955036/168512311-a3b074f7-e7f4-4638-8744-2731e48c953b.png)
# FLOWCHART
![FLOWCHART](https://user-images.githubusercontent.com/94955036/168512312-39a8bf6d-cb8e-46c2-a61b-60a28eb4c8cd.png)
# PIN DIAGRAM
![PIN DIAG](https://user-images.githubusercontent.com/94955036/168512317-ba649a27-9bca-4634-b466-dbeebeac8a12.png)
# STM32F407VG BOARD
![ST DISC KIT](https://user-images.githubusercontent.com/94955036/168512323-05f3dc12-a3fb-42ce-b704-8b2c561e7687.png)

