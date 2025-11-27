---
{"dg-publish":true,"permalink":"/guides-references-and-troubleshooting/misc/st-ps-and-sumps/stp-relay/ref-gilbarco-isolation-relay/"}
---


![IsoRelay1.jpeg](/img/user/Assets/Images/IsoRelay1.jpeg)

This device receives a hook signal from multiple devices and trips a relay that delivers power to the STP relay.  

![IsoRelay2.jpeg](/img/user/Assets/Images/IsoRelay2.jpeg)

Hook signal and a matching neutral lands on the same numerical landing on the right.  That closes a small relay closes then fires the big relay on the left.  

![IsoRelay3.jpeg](/img/user/Assets/Images/IsoRelay3.jpeg)

PO is the relay coil.  When power is applied, the relay closes and the STP activates.  

PI is the signal wire.  Power comes from L1 and is let through to PI by the hook signal isolation bank.  PI will send the L1 power to anywhere you want to “know when a hook signal comes in”.  

You can always jumper PI and PO to automatically activate the relay when a hook signal comes in.  