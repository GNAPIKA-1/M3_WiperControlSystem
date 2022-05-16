***Wiper Control System***
## Objective:
In this project, a high-performance **Arm® Cortex®-M4 32-bit RISC core**, STM32F407VG Microcontroller Board is used to demonstrate the working of ***Wiper Control System*** of an automobile at different states of modes and positioning the Wiper.
## Brief Explanation of Project:
>![illustration](https://user-images.githubusercontent.com/94955036/168634920-deb273a9-1d9f-4ab3-9c79-b9e6bf49c969.png)
>The second position switch of key in Automobile, is the **ACC/ACCESSORY position, which allows you to use your radio, windshield wipers**, and other accessories while the engine is off. This position should also be used in the event that your vehicle is being pushed or towed. In this position, the engine is off.(The next one is the ignition position. All the electronic accessories come active when you turn on the ignition switch in this mode. According to the expert maintenance tips, the ***ON position*** is the default position in vehicles.)
### Working:
In this project, we are enhancing the speed and frequency rate of Wiper and ensuring it in the correct position, so that Driver, catches the view of sight perfectly.Here, the LEDs of STM32F407VG Microcontroller are considered as Position of Wiper.Blue, Green and Orange are the LEDs.Alternately, the rate of frequency is taken from ON and OFF process to set frequency.When the PUSH Button is clicked Red LED will be ON.
#### Scenario:
- ***Ignition Key Position at ACC***: The Red LED is ON, if the user button is pressed and held for 2 secs
- ***Wiper ON: Wiper is OFF***: On press of the user input, Blue, Green and Orange LEDs come ON one at a time with the set frequency, The frequency changes on every alternate key press, 3 frequency levels with 1, 4 and 8 Hz
- ***Wiper OFF: Wiper is ON:*** The LED glow pattern stops on the 4th press; the wiper action starts next press onwards as mentioned in step 2
- ***Ignition Key Position at Lock***: The Red LED is OFF, if the user button is pressed and held for 2 secs

![work](https://user-images.githubusercontent.com/94955036/168655361-950b9164-23a7-47c9-939b-50ecc89e0a71.png)

#### Different States of Mode:
| MODES  | CONDITION |
| ------------- | ------------- |
| MODE 1  |  Red LED is ON |
| MODE 2  |  Blue, Green and Orange LEDs ON at 1Hz  |
| MODE 3  |  Blue, Green and Orange LEDs ON at 4Hz   |
| MODE 4  |  Blue, Green and Orange LEDs ON at 8Hz   |
| MODE 5  |  Red LED is OFF |

### COMPONENT
***STM32F407VG MICROCONTROLLER BOARD***
![This is an image](https://robu.in/wp-content/uploads/2018/07/STM32F407-Discovery-Kit-for-STM32F407Robu-2.jpg)
>The STM32F405xx and STM32F407xx family is based on the high-performance Arm® Cortex®-M4 32-bit RISC core operating at a frequency of up to 168 MHz.
The Cortex-M4 core features a Floating point unit (FPU) single precision which supports all Arm single-precision data-processing instructions and data types. 
It also implements a full set of DSP instructions and a memory protection unit (MPU) which enhances application security. 
The STM32F405xx and STM32F407xx family incorporates high-speed embedded system.


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

# BLOCK DIAGRAM
![BLOCK DIAGRAM](https://user-images.githubusercontent.com/94955036/168512298-81fc8a9d-74ba-424b-9510-a5de305e2701.png)

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

# Output Video:


https://user-images.githubusercontent.com/94955036/168659743-879f6863-2014-4657-981f-2e18d0011df7.mp4

***From above output video, we can see, a Red LED, will be ON, i.e; after pressing user button long, for 2sec, which indicates the start of engine, where Wiper gets ready from still state to stimulate. Then, pressing user button again, leads to run of Blue, Green and Orange LED's, blinking one by one at certain frequency, for every time button is pressed, it increases the speed of blinking rate from start position to end, going from Blue LED to Orange LED and vice-versa, crossing Green LED, where this LEDs indicates, position of Wiper that is moving at different scenario, when user button is preesed again and again.To stop, and bring the Wiper at initial state, long press of user button, makes control system in OFF state.***

![Code Score](https://api.codiga.io/project/33440/score/svg)

![Code Grade](https://api.codiga.io/project/33440/status/svg)
