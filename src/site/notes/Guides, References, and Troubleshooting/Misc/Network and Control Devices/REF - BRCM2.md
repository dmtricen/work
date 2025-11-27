---
{"dg-publish":true,"permalink":"/guides-references-and-troubleshooting/misc/network-and-control-devices/ref-brcm-2/"}
---

## Basics

The job of the BRCM2 is to translate the messages sent by the DCM on the dispensers into information that can be understood by the FCI or put on the local network to the fuel controller via TCP/IP.  
It is made up of three components (only 2 on the newest version).

---
## Components

### Field Wiring Board

![BRCM2-2 1.jpeg](/img/user/Assets/Images/BRCM2-2%201.jpeg)

This takes the wiring from the dispensers and splits the signal into pump and crind signals.  The crind is sent to the front lid of the BRCM2 to head out on the network and the pump is wired over the top of the back plate to the DBox board. 

### DBox Board

![BRCM2-3.jpeg](/img/user/Assets/Images/BRCM2-3.jpeg)

Sends pump signals to the FCI for processing.  The red leds light up on a channel that expects to see data but isn't receiving data.  

### Lid


The front of the BRCM2 actually has a DCM inside translating the traffic before being put on the network. 

---


Some have an extra port labeled “2” left of the bank of ports.  It has no rxtx lights.  DONT USE IT.

Only use bank of ports

![BRCM2.jpg](/img/user/Assets/Images/BRCM2.jpg)

![Assets/Images/BRCM2-2.jpeg](/img/user/Assets/Images/BRCM2-2.jpeg)

