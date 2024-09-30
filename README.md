# DSpeed
Speeduino incarnation based on ATMega2560 with some extra features.

## Configuration jumpers

| ID | Function | Description |
| :---: | :---: | --- |
| J1 |      |     |
| J2 | O2    | Jumping 1-2 feeds the Speeduino with the external O2 Sensor input signal. Jumping 2-3 feeds the Speeduino with the signal from the build in wide band oxygen sensor controler. |
| J3 | Crank | Must be ON together with J6 when internal conditioner for Crank position sensor is used. Must be OFF together with J6 when external conditioner is used. |
| J4 | Cam   | Must be ON together with J5 when internal conditioner for Cam position sensor is used. Must be OFF together with J5 when external conditioner is used. |
| J5 | Cam   | Must be ON together with J4 when internal conditioner for Cam position sensor is used. Must be OFF together with J4 when external conditioner is used. | 
| J6 | Crank | Must be ON together with J3 when internal conditioner for Crank position sensor is used. Must be OFF together with J3 when external conditioner is used. |
| J7 | MAP   | Jumping 1-2     |
| J8 | Crank | When ON a 10k pull-up resistor to 5V is added on Crank position sensor input. |
| J9 | Cam   | When ON a 10k pull-up resistor to 5V is added on Cam position sensor input. |
| J10 | VSS  | Jumping 2-3 adds a 10k pull-up resistor to 5V on Vehicle Speed Sensor input. USed for sensors with an open collector output pulling signal to ground only such us some Hall sensors. Jumping 1-2 adds a 270R pull-down on Vehicle Speed Sensor input. Used for 2-wire Hall sensors where signal is mixed with power as found in some ABS systems. For VR sensors leave jumper open. |
| J11 |        |      |
| J12 |        |      |
| J13 |        |      |
| J14 |        |      |
| J15 | Crank  | When ON the Crank- input is internally shortenned to ground. Should be ON when using VR sensor with internal conditioner and it is not grounded elswhere. |
| J16 | Cam    | When ON the Cam- input is internally shortenned to ground. Should be ON when using VR sensor with internal conditioner and it is not grounded elswhere. |
