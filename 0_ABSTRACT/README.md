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
## Structure:

## Software Used:
