---
{"dg-publish":true,"permalink":"/troubleshooting/point-of-sales/pinpads/mx-900-pinpad/"}
---

*A pdf related to this entry is available.  Refer to [[Troubleshooting/Manuals and Guides\|Manuals and Guides]] for a link.*

[[MX900 Pinpad.pdf]]

This thing is older and temperamental, so these are the methods I used to install these pin pads in the past.  You may need to call Verifone if it goes pear shaped.  

Step 1) 
   - Identify the file versions you will need.  
   - Find out what version software they are running on the commander and look up the service document for that software.  Inside you’ll find the versions of the software you need for the OS and Viperpay.  
   - NOTE: As of writing this, there is only one version of Contactless software.  That may change.  It wasn’t referenced in the service document when I checked
   - NOTE: I couldn’t find the service document for the version software on the commander the last time I did this.  I chose a close version and it resulted in the Viperpay software version being too old.  Be aware of this. 

Step 2) 
   - Take a picture of the back of the new pin pad (with the serial number) and send an email to dispatch including the site name, store brand name, and ticket number and ask for encryption to be ordered.  They will send an email when it’s done.  

Step 3) 
   - Download the appropriate version of:
	   - the Pinpad OS (Verifone website)
	   - Viperpay (Verifone website)
	   - Contactless software (Verifone website)
	   - Encryption (Verifone through email)

Step 4) 
   - get your hands on the support number for the brand.  You will likely have to call them to whitelist the pin pad. 

Step 5) 
   - load the configuration mode and record the ip address of the pin pad.  Physically install the pin pad but don’t plug in the Ethernet cable! ( it could interfere with any other pin pads ).  

Step 6)
   - Download all four software files to usb (in .tgz format as the pin pad will not load a usb with anything else on it INCLUDING folders)

Step 7)
   - Install usb into pin pad and load configuration mode (hit 1, 5, and 9 simultaneously).  Go to administration tab then to transfer and then usb.  Load each file one at a time and restart the unit between.  The OS makes it restart to the Verifone screen multiple times before being done.  

Step 8)
   - Once done, go into configuration mode and change the up address to the right one (default is fine if there is only one but you might have to increment the final number if there are more.)

Step 9) 
   - The port needs to be changed from 4000 to 5000.  To do this, wait till the pin pad shows the welcome screen and tap the two invisible buttons on the bottom right of the screen back and forth until you enter Viperpay config.  Here you can change the port.

Step 10) 
   - Restart the pin pad and plug in the Ethernet cable.  Once it’s up, log into the commander and reinitialize the emv (select the pin pad in question and add it to the selected group and log off).  

Step 11) 
   - Log off the POS and log back in after the pin pad comes all the way up.  Attempt to make a transaction.  It might cause the pin pad to restart.  That’s ok.  Test both insert and contactless.  


Install files in the following order: 

1) OS
2) Viperpay
3) Contactless
4) Encryption 

Check the release notes for the commander version the site is running to know what version each software to install

NOTE: the usb you use to install software must be fat32 formatted and must not contain any folders or non-tgz extension files or it won’t mount. 

Don’t forget to whitelist the new pin pad with the brand.  