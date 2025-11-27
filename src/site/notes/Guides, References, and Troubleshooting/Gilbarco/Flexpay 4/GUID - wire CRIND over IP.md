---
{"dg-publish":true,"permalink":"/guides-references-and-troubleshooting/gilbarco/flexpay-4/guid-wire-crind-over-ip/"}
---

![DCM3.jpeg](/img/user/Assets/Images/DCM3.jpeg)

The Blue/ Yellow pair is normally CRIND and the Red/Yellow is pump.  With CRIND over IP and a DCM3, wire the twisted pair (likely the wires they used for CRIND) to the Yellow/Yellow pair going to the DCM3 and ignore the Blue/Yellow coming from the Omnia Board.  

Ultimately it goes to the BRCM2 for data splitting.  