---
{"dg-publish":true,"permalink":"/troubleshooting/leak-detection/veeder-root/plld-setup-on-a-tls-450-plus/"}
---


This continuing education bulletin provides information to Veeder-Root certified technicians how to setup PLLD on the TLS-450PLUS  

Console Requirements:

To run PLLD tests the console must have the PLLD feature loaded onto the consoles iButton. Also, the console must have a Pump, Line setup to run in Pump control mode.

Setup:

1. Wiring: 120VAC and a Neutral must be brought to each I/O Card in the console

a. Each PLLD sensor is wired to the consoles USM

b. External Input: the dispenser hook signal for a product is wired to one terminal of a E/I port on the I/O card. The other terminal is tied to neutral.

c. Relay: One terminal of the relay is wires to A High-Power Relay which will energize the STP. The other terminal is wired to 120VAC.

![PLLD1.png](/img/user/Assets/Images/PLLD1.png)
2. Setup Devices

a. Relay:

i. Configured Enabled

ii. Select address: Bx.SX.5-9

iii. Enter a Label

iv. Type: Pump control

v. Orientation: Normally open

b. External Input: 

i. Configured: Enabled

ii. Select Address: BX.SX.10 – 14

iii. Enter a Label

iv. Type: Pump Sense

v. Orientation: Normally Open

c. Line Pressure Sensor:

i. Configured: Enable

ii. Select Address on USM

iii. Enter a Label

Hit the Home Button, then Menu/Setup/Pumps & Lines/Pump

3. Setup Pump

a. Configured: Enable

b. Enter a Label

c. Mode: TLS: Pump Control

d. Tank: select Tank 

e. Pump Control: select relay for the product

f. Pump Sense: select external input for the product dispenser signal

![PLLD2.png](/img/user/Assets/Images/PLLD2.png)

Hit the Arrow next to Pump at the top of the screen, select Line

4. Setup Line

a. Configure: Enable

b. Enter a Label

c. Leak Monitoring: Monitoring PLLD

d. Pressure Sensor: select LPR for the product

e. Selected Pumps: slide desired pump from Available Pumps

![PLLD3.png](/img/user/Assets/Images/PLLD3.png)

Hit the arrow next to Line, select PLLD

5. Setup PLLD

a. Configured: Enabled

b. Select Pipe Type

c. Enter piping length referencing the pipes diameters

d. 0.2gph Line Leak: select how often the test will run

e. 0.1gph Line Leak: select how often the test will run

f. Shutdown Rate: select rate required by regulations

g. Low Pressure Shutoff: Enabled

h. Low Pressure Alarm Limit (psi): 10

i. Continuous Handle Timeout (Hr): 16

j. Fuel Out Limit (in): 10

![PLLD4.png](/img/user/Assets/Images/PLLD4.png)

![PLLD5.png](/img/user/Assets/Images/PLLD5.png)

![PLLD6.png](/img/user/Assets/Images/PLLD6.png)

6. Perform a Manual Gross Test to enable the line


