---
{"dg-publish":true,"permalink":"/troubleshooting/gilbarco-dispenser-architecture/"}
---

Gilbarco dispensers are made up of two major systems, the Card Reader in Display (CRIND) and the Pump.  Both communicate with different things inside and usually communicate with each other inside the dispenser.  

---
### CRIND

This system is made up of everything you’d need to pay at the pump.  
- Flex pay architecture (2 or 4)
- Invenco architecture 

This is usually the screen, the UPM (pinpad), card reader, the CRIND logic board like OMNIA or SSOM, and the board that interprets data coming from inside called the DCM.  


---
### Pump

This system involves stuff you need to go inside and prepay for gas.  This includes the pump control node, the door display boards, the PPUs, and everything in the lower cabinet of the dispenser.  

---
### Communications

The CRIND logic board and the pump control node are usually connected so that the CRIND can turn on the pump in the event of outside card sales.  The DCM (dispenser communication module) is responsible for receiving instructions from the BRCM2 and ultimately from the fuel controller over tcp/ip.  The pump control node gets instructions from the FCI and ultimately from the fuel controller on a direct connection.  

---
