---
{"dg-publish":true,"permalink":"/troubleshooting/network-and-control-devices/brcm-2/","tags":["Keep/Color/Purple","Keep/Attachment","Keep/Label/Troubleshooting-Guide"]}
---

## Basics

The job of the BRCM2 is to translate the messages sent by the DCM on the dispensers into information that can be understood by the FCI or put on the local network to the fuel controller via TCP/IP.  
It is made up of three components (only 2 on the newest version).

---
## Components

### Field Wiring Board

![IMG_2668.jpeg](/img/user/Assets/IMG_2668.jpeg)

This takes the wiring from the dispensers and splits the signal into pump and crind signals.  The crind is sent to the front lid of the BRCM2 to head out on the network and the pump is wired over the top of the back plate to the DBox board. 

### DBox Board

![IMG_2669.jpeg](/img/user/Assets/IMG_2669.jpeg)

Sends pump signals to the FCI for processing.  

### Lid


The front of the BRCM2 actually has a DCM inside translating the traffic before being put on the network. 

---


Some have an extra port labeled “2” left of the bank of ports.  It has no rxtx lights.  DONT USE IT.

Only use bank of ports

![BRCM2.jpg](/img/user/Assets/Images/BRCM2.jpg)

![BRCM2-2.jpeg](/img/user/Assets/Images/BRCM2-2.jpeg)

