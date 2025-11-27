---
{"dg-publish":true,"permalink":"/guides-references-and-troubleshooting/gilbarco/dispensers-and-pumps/encore/ref-encore-700-programming/"}
---

*A pdf related to this entry is available.  Refer to [[Guides, References, and Troubleshooting/Misc/REF - Manuals and Guides\|REF - Manuals and Guides]] for a link.*

[[encore 500&700 pump programming.pdf]]

---

91 - 49 - Nozzle Guard
	5 - this sets it to “uses crind”

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
# Selects Grade w/o Button

In the case you have an encore and it auto selects a grade instead of letting you press a button (I’ve only seen this happen on single product pumps), you correct this behavior with CC 91.  

FC 2 and FC 12 are defaulted to 1.  The only other option for either of those is 2.  Try different combinations of those function codes and see which one will let you press the button.  In my case, I needed FC 12 to be 2 and FC 2 to be default 1.  