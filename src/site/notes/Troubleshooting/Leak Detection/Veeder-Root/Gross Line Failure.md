---
{"dg-publish":true,"permalink":"/troubleshooting/leak-detection/veeder-root/gross-line-failure/"}
---


### Troubleshooting

During a gross test, the pump turns on and the console records the pressure (Pon). Then, the pump turns off and two additional pressure readings (P1 and P2) are recorded. If the pressure drops below 12 psi, the gross line test fails, and an alarm will be displayed.

- Check for visible leaks – STP sump and under all dispensers.
- Verify the tank is not out of fuel. An empty tank will prevent a line from properly pressurizing.
- Check for other alarms on the console. Depending on console programming, other alarms might prevent a manual gross line test from running.
- Check the line’s pressure.

### Accessing PLLD Records

#### - TLS-450PLUS

Menu > Diagnostics > PLLD > 3.0 gph Tests  
This screen displays the five most recent passes and five most recent fails per line.

#### - TLS-350

1. Press MODE for DIAG MODE
2. FUNCTION to PRESSURE LINE LEAK DIAG
3. STEP to 3.0 DIAG
4. Press PRINT

The printout will display the five most recent passes and fails for the line selected.

- Run a manual gross line test.

### Troubleshooting Examples:

![PLLD Gross line failure examples](https://www.veeder.com/us/sites/veeder.com.us/files/inline-images/TSN-Gross-Line-Failure-Examples.jpg)

#### Possible Causes for Each Example:

|                                                                                                                                                                                                                                                                                                    |                                                                                                                                                                                                                                                                                                       |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Example 1**<br><br>- Line leak<br>- Incorrect programming - line type or line length<br>- Bad check valve<br>- Bad blender valve<br>- Bad dispenser valve<br>- Bad air purge screw (The Red Jacket)<br>- Bad SwiftCheck valve (Standard Red Jacket)<br>- Bad packer o-ring (Standard Red Jacket) | **Example 2**<br><br>- Tripped circuit breaker<br>- Relay is not activating/Pump is not turning on<br>- Bad starting capacitor<br>- Bad ump<br>- Out of fuel<br>- Catastrophic leak (worst case)                                                                                                      |
| **Example 3**<br><br>- Air in the line<br>- Sticky pump control relay<br>- Bad pressure relief check valve (The Red Jacket)<br>- Partially clogged functional element or vent path (Standard Red Jacket)                                                                                           | **Example 4**<br><br>- Blender valve leaking<br>- Bad air purge screw (The Red Jacket)<br>- Faulty check valve (The Red Jacket or Standard Red Jacket)<br>- Bad packer o-ring (Standard Red Jacket)<br>- Bad SwiftCheck valve (Standard Red Jacket)<br>- Dispenser - bad handle signal or drive board |
