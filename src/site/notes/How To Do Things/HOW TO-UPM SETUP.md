---
{"dg-publish":true,"permalink":"/how-to-do-things/how-to-upm-setup/","tags":["Keep/Color/Purple","Keep/Attachment","Keep/Label/Troubleshooting-Guide"]}
---


Initial setup for UPMs

————————————————————————

[[Flexpay IV CRIND.pdf]]


![UPM.jpg](/img/user/Assets/Images/UPM.jpg)

---

# Steps to Replacing a UPM

1. If the old UPM will let you into setup, print out a setup config
2. Remove the old UPM.  I recommend turning it over and placing it beside the new UPM and taking a picture of both serial numbers.  It’ll help later. 
3. Install new UPM.
4. Turn dispenser on and quickly take a picture of the screen to get the UPM serial number (otherwise you have to read it off the sticker on the UPM which can be difficult).
5. Wait for the “1) setup” prompt to appear in the bottom left hand corner of the white screen.  This may take a while, especially if the yellow “Secure Update” square appears.  That can take up to 10 min to finish.  Once it appears, hit 1 on the UPM keypad. 
6. The password to enter setup is the last 6 digits of the serial number.  You have a picture of it.

Instructions diverge here depending on what hardware you have.  

---
# …If you have an Omnia board
1. ****Change device to Omnia
2. Restart the dispenser and reenter setup
3. Enter secure menu with option 8
4. Activate all devices with option 3


---
# …if you have an SSOM on a CCP
1. *Change device settings option 2 
2. *Change ip address and ensure the mask and gateway match other dispensers
3. Back to main menu
4. Enter secure menu with option 8
5. Activate all devices with option 3


---
# Installing Encryption (RKLs)
1. Make sure your laptop has internet access
2. Connect to the UPM with the UPM Maintenance tool
3. Click RKL
4. On your phone, open the Gilbarco activation app
5. Login and click RKL
6. Select your site and choose flex pay 4
7. Enter the serial and hash displayed on your laptop
8. Select the RKL needed.
9. It will send a password to your text messages.  Copy the password and enter it into the Gilbarco activation app. 
10. *It’s ready!  Click go.  Once it’s done, check the setup print out to ensure it’s listed at the bottom



---




![CertsFigure1.jpeg](/img/user/Assets/Images/CertsFigure1.jpeg)

*Note*: “Loading Monochrome” is an indication that the site is using a Passport and that the UPM is NOT communicating with the EDH.  You must load the rcsh certificate (through tac) to fix.  Must do this every time UPM changes on a Passport site. Also, check your IP addresses.  Is the gateway x.x.x.254?

*Note:* You must call Gilbarco to do a rcsh download.  You can’t do it through the app. They call this a “TLS Certificate Download”.
