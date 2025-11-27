---
{"dg-publish":true,"permalink":"/guides-references-and-troubleshooting/gilbarco/flexpay-4/trbl-ux-300-card-readers/"}
---




---

## Troubleshooting


#### Card Reader Errors

![image000000.jpeg](/img/user/Assets/Images/image000000.jpeg)

SB2990 Contains all the error codes and what to do about them.  It is a living document.

#### Card Reader Activation on a DCM2 w/o SSOM

Normally activating card readers is a straight forward process, but if you have a DCM2 with no SSOM, you are supposed to disable the entire opposite side before trying.  If you don't, you'll have issues like the card reader not responding when you press the button on the back.  However, to avoid all that, you can unplug the ethernet cable from both the card reader and the UPM.  Then take your own ethernet cable and plug one side into the card reader and the other end into the UPM.  Then activate like normal!  