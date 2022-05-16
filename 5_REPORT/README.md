# ABSTRACT
## Project Name:
***Wiper Control System***
## Objective:
In this project, a high-performance **Arm® Cortex®-M4 32-bit RISC core**, STM32F407VG Microcontroller Board is used to demonstrate the working of ***Wiper Control System*** of an automobile at different states of modes and positioning the Wiper.
## Brief Explanation of Project:
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
# SOFTWARE REQUIREMENTS

* STM32 IDE
* QEMU


# COMPONENTS
* STM32F407VG MICROCONTROLLER BOARD


# REQUIREMENTS DESCRIPTION:
## STM32F407VG
* The STM32F405xx and STM32F407xx family is based on the high-performance Arm® Cortex®-M4 32-bit RISC core operating at a frequency of up to 168 MHz.
*  The Cortex-M4 core features a Floating point unit (FPU) single precision which supports all Arm single-precision data-processing instructions and data types. 
*  It also implements a full set of DSP instructions and a memory protection unit (MPU) which enhances application security. 
*  The STM32F405xx and STM32F407xx family incorporates high-speed embedded system.


## Xpack Packages :

### Windows Build Tools: 
* The xPack Windows Build Tools is a standalone Windows binary distribution of GNU make and a few of other tools required by the Eclipse Embedded CDT (formerly GNU MCU/ARM Eclipse) project, but the binaries can also be used in generic build environments.
### OpenOCD :
* Open On-Chip Debugger (OpenOCD) is a free, open-source project that aims to provide debugging, in-system programming, and boundary scan using a debug adapter. 
* The adapter is a hardware module that provides the right signals for the target to understand.


### QEMU :
* The xPack QEMU Arm is a standalone cross-platform binary distribution of QEMU, with several extensions for Arm Cortex-M devices.


# FEATURES OF STM32F407VG MICROCONTROLLER
### Memories
* Up to 1 Mbyte of Flash memory.
* Up to 192+4 Kbytes of SRAM including 64-Kbyte of CCM (core coupled memory) data RAM.
* 512 bytes of OTP memory.
* Flexible static memory controller supporting Compact Flash, SRAM, PSRAM, NOR and NAND memories.
### Clock, reset and supply management
* 1.8 V to 3.6 V application supply and I/Os
* POR, PDR, PVD and BOR
* 4-to-26 MHz crystal oscillator
* Internal 16 MHz factory-trimmed RC (1% accuracy)
* 32 kHz oscillator for RTC with calibration
* Internal 32 kHz RC with calibration
### Low-power operation
### 3×12-bit, 2.4 MSPS A/D converters: up to 24 channels
### 2×12-bit D/A converters
### Upto 17 timers,etc

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

## Structure:

## Software Used:
**STM32 IDE** -STMicroelectronics' STM32 family of 32-bit ARM Cortex-M core-based microcontrollers is supported by a wide range of software integrated development environments (IDEs) with C, C++, Pascal and JAVA support and debuggers from STMicroelectronics, allowing to configure and initialize the MCU or monitor its behavior in run time.

**QEMU** -It emulates the machine's processor through dynamic binary translation and provides a set of different hardware and device models for the machine, enabling it to run a variety of guest operating systems.
# DESIGNS
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
## High Level Test Cases
|TEST CASES| EXPLANATION |INPUT| OUTPUT|RESULT| STATE |
| :-----|:-----------|:------------|:------------|:------------|:------------|
|HL01|check if the BUTTON is pressed|program execution|Microcontroller/Engine starts|LED ON(RED)| PASS|
|HL02|check if the BUTTON is pressed|program execution|	WIPER starts|LED ON(BLUE)| PASS|
|HL03|check if the BUTTON is pressed|program execution|	WIPER starts|LED ON(GREEN)| PASS|
|HL04|check if the BUTTON is pressed|program execution|	WIPER starts|LED ON(ORANGE)| PASS|
|HL05|check if the BUTTON is pressed|-|Microcontroller/Engine stops|LED TURNED OFF| PASS|

## Low Level Test Cases

|TEST CASES| EXPLANATION |INPUT| OUTPUT| RESULT |STATE |
| :-----|:-----------|:------------|:------------|:------------|:------------|
|LL01|check if the BUTTON is pressed|program execution|Microcontroller/Engine starts|LED ON(RED)| PASS|
|LL02|check if the BUTTON is pressed|program execution|WIPER starts and speed of wiper is slow	|LED ON(BLUE)| PASS|
|LL03|check if the BUTTON is pressed|program execution|WIPER starts and speed of wiper is moderate	|LED ON(GREEN)| PASS|
|LL04|check if the BUTTON is pressed|program execution|WIPER starts and speed of wiper is good|LED ON(ORANGE)| PASS|
|LL05|check if the BUTTON is pressed|-|Microcontroller/Engine stops|LED TURNED OFF| PASS|

