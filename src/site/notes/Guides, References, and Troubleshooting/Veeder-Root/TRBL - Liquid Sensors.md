---
{"dg-publish":true,"permalink":"/guides-references-and-troubleshooting/veeder-root/trbl-liquid-sensors/"}
---


---

# Troubleshooting Connections

On basically any tank monitor, you’ll have a diagnostic screen that looks like this
![LiquidSensorDiag1.jpeg](/img/user/Assets/Images/LiquidSensorDiag1.jpeg)
**Value** represents the amount of resistance in Ohms that is on that circuit.  That number is usually how the tank monitor knows when the device should go into alarm. 

**Sample Counter** is unique to Veeder-Root, I believe.  It tells you how many successful sample tests it has done of the device in a row (max of 5).  If that is fluctuating down to 1 and counting up a lot, then that indicates you probably have bad field wiring, because some of its tests keep coming back negative.  

---
