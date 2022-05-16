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
