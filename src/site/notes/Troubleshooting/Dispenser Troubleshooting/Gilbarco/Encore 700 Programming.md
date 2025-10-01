---
{"dg-publish":true,"permalink":"/troubleshooting/dispenser-troubleshooting/gilbarco/encore-700-programming/","tags":["Keep/Color/Purple","Keep/Attachment","Keep/Label/Troubleshooting-Guide"]}
---


---

[[encore 500&700 pump programming.pdf]]

---

91 - 49 - no idea
	5 - 

90 - Type of pump
—— 1 -  1 product 1 hose
—— 13 - 3 product 1 hose blender
—— 6   - 3 product straight grade
—— 17 - 3 grade 1 hose blender +1

82 - Calibration can size
	5 - Five gallons

72 - blend ratios (must use security switch)
	(100, 65, 0)

71 - Volume unit type
	1 - US Gallons

49 - Prestarts
	1 - 2
	2 - 1

20 - Prices {top # is side (3 is both sides)}
        First sub # is grade (1-6)

40 - Pump Numbers
	1 - is A-side (with security switch)
	2 - is B-side
         (Leave on 7&11 when using passport)

---

80 - Max Flow (default 10 gallons)
	1 - side A
	2 - side B
	change to 98 for high flow

96 - Dispenser Model
	5 - 500 S
	7 - 700 S

92 - Sides
	 1 - Both sides exist


![CommonProgramming.jpg](/img/user/Assets/Images/CommonProgramming.jpg)


---
# High Flow Diesel Issues

Does the flow suddenly stop and go?   Check code 80 Max Flow.  You’ll find it’s at default.  Needs to be 98.

---
# Encore Flow Rate

Once 2 gallons of fuel have been dispensed, press the #5 key on the manager’s keypad, on the money/volume display, the monetary value will be replaced with the current gallons per minute the dispenser is clocking in – this works when the dispenser is in standalone as well as in normal operating mode and will work on high flow diesels as well. For best results, dispense at least 5 gallons of fuel WITHOUT slowing the flow rate down or having the nozzle click off.

---
