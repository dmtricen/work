---
{"dg-publish":true,"permalink":"/guides-references-and-troubleshooting/gilbarco/flexpay-4/trbl-fpiv-crind-communications/"}
---

## CRIND BIOS

When a Flexpay IV dispenser can’t communicate with the fuel controller (be it commander, dex, etc.) it will stop loading on the screen showing “crind bios”.  I haven’t found any way to fix this without restarting the fuel controller.  This usually involves a call to 7-11, verifone, or Gilbarco.  Or, you could manually restart it.  

---
## Loading Monochrome

In a MOC environment (aka using a Passport), if the crind can't communicate with the EDH for any reason, it will get stuck on this message.  To resolve this...

- Check your wiring
	- I would connect to the Omnia/SSOM and try to ping the gateway.  Or you can connect to the BRCM2 and try to ping the dispenser.  If it's successful, your wiring is good.
- Check your PCN programming
	- using the managers keypad, use Command Code 40, Function Codes 1&2 and make sure that they are 7&11.  
- Check your UPM programming
	- Using your blue card, check and make sure that the number under Pump is 7 on side A and 11 on side B.
- Check Omnia/SSOM programming
	- login with your laptop and ensure it is ALSO 7&11 for sides A and B.

---
## Loading Application 

In an MOC environment (aka, using Passport), if the crind can't communicate with the PCN, it will stick at this screen.  To resolve this...

- Verify dispenser is not in bypass
- Verify the 2-wire is plugged into both the PCN and the Omnia/CCP.  
- Verify your getting data transmitted to the PCN via the tx/rx LEDs.
