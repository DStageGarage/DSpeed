# DSpeed
Speeduino incarnation based on ATMega2560 with some extra features.

## Configuration jumpers

| ID | Function | Description |
| :---: | :---: | --- |
| J1 | Ignition | Jumping 1-2 sets the cooil drivers voltage to 5V. Jumping 2-3 sets the cooil drivers voltage to 12V. For use with built-in ignition transistors (passive coils set witj J11-14) use of 12V may result in less heat dissipated in transistors although it may be case dependant and both settings will work. For active coils (set with J11-14) user has to know which input voltage is correct for them. |
| J2 | O2    | Jumping 1-2 feeds the Speeduino with the external O2 Sensor input signal. Jumping 2-3 feeds the Speeduino with the signal from the built-in wide band oxygen sensor controler. |
| J3 | Crank | Must be ON together with J6 when internal conditioner for Crank position sensor is used. Must be OFF together with J6 when external conditioner is used. |
| J4 | Cam   | Must be ON together with J5 when internal conditioner for Cam position sensor is used. Must be OFF together with J5 when external conditioner is used. |
| J5 | Cam   | Must be ON together with J4 when internal conditioner for Cam position sensor is used. Must be OFF together with J4 when external conditioner is used. | 
| J6 | Crank | Must be ON together with J3 when internal conditioner for Crank position sensor is used. Must be OFF together with J3 when external conditioner is used. |
| J7 | MAP   | Jumping 1-2 connects the built-in MAP sensor to Speeduino A5 input while external source remains connected to A3 input. This allows for using one for atmospheric compensation. Jumping 2-3 sets the use of built-in MAP sensor only by conecting it to Speeduino A3 input. External sensor signal input should remain unconnected in this case!    |
| J8 | Crank | When ON a 10k pull-up resistor to 5V is added on Crank position sensor input. |
| J9 | Cam   | When ON a 10k pull-up resistor to 5V is added on Cam position sensor input. |
| J10 | VSS  | Jumping 2-3 adds a 10k pull-up resistor to 5V on Vehicle Speed Sensor input. USed for sensors with an open collector output pulling signal to ground only such us some Hall sensors. Jumping 1-2 adds a 270R pull-down on Vehicle Speed Sensor input. Used for 2-wire Hall sensors where signal is mixed with power as found in some ABS systems. For VR sensors leave jumper open. |
| J11 | Ignition | For COIL1 output. Jumping 1-2 sets the "passive coil" option meaning the output is controled with a built-in transistor. Jumping 2-3 sets the "active coil" option meaning a 5/12V (see J1 setting) logic signal at the output. |
| J12 | Ignition | For COIL2 output. Jumping 1-2 sets the "passive coil" option meaning the output is controled with a built-in transistor. Jumping 2-3 sets the "active coil" option meaning a 5/12V (see J1 setting) logic signal at the output. |
| J13 | Ignition | For COIL3 output. Jumping 1-2 sets the "passive coil" option meaning the output is controled with a built-in transistor. Jumping 2-3 sets the "active coil" option meaning a 5/12V (see J1 setting) logic signal at the output. |
| J14 | Ignition | For COIL4 output. Jumping 1-2 sets the "passive coil" option meaning the output is controled with a built-in transistor. Jumping 2-3 sets the "active coil" option meaning a 5/12V (see J1 setting) logic signal at the output. |
| J15 | Crank  | When ON the Crank- input is internally shortenned to ground. Should be ON when using VR sensor with internal conditioner and it is not grounded elswhere. |
| J16 | Cam    | When ON the Cam- input is internally shortenned to ground. Should be ON when using VR sensor with internal conditioner and it is not grounded elswhere. |
