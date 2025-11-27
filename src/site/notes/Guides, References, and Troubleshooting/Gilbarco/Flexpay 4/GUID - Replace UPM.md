---
{"dg-publish":true,"permalink":"/guides-references-and-troubleshooting/gilbarco/flexpay-4/guid-replace-upm/"}
---


*A pdf related to this entry is available.  Refer to [[Guides, References, and Troubleshooting/Misc/REF - Manuals and Guides\|REF - Manuals and Guides]] for a link.*

## Initial setup for UPMs

————————————————————————

[[Flexpay IV CRIND.pdf]]


![UPM.jpg](/img/user/Assets/Images/UPM.jpg)

---

## Steps to Replacing a UPM

1. If the old UPM will let you into setup, print out a setup config
2. Remove the old UPM.  I recommend turning it over and placing it beside the new UPM and taking a picture of both serial numbers.  It’ll help later. 
3. Install new UPM.
4. Turn dispenser on and quickly take a picture of the screen to get the UPM serial number (otherwise you have to read it off the sticker on the UPM which can be difficult).
5. Wait for the “1) setup” prompt to appear in the bottom left hand corner of the white screen.  This may take a while, especially if the yellow “Secure Update” square appears.  That can take up to 10 min to finish.  Once it appears, hit 1 on the UPM keypad. 
6. The password to enter setup is the last 6 digits of the serial number.  You have a picture of it.
7. Follow the Flexpay IV CRIND guide for normal settings.  

Instructions diverge here depending on what hardware you have.  

---
## …If you have an Omnia board
1. ****Change device to Omnia
2. Restart the dispenser and reenter setup
3. Enter secure menu with option 8
4. Activate all devices with option 3


---
## …if you have an SSOM on a CCP
1. *Change device settings option 2 
2. *Change ip address and ensure the mask and gateway match other dispensers
3. Back to main menu
4. Enter secure menu with option 8
5. Activate all devices with option 3


---
## Installing Encryption (RKLs)
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
## Troubleshooting

#### Loading for a Passport site

If the UPM is connecting to a Passport, you have to load a "TLS Certificate" so that they can communicate.  Use the M7 Maintenance Tool and click "RCSH Download".  From here, you have to call Gilbarco and ask for a "TLS Certificate Download".  From here, it's similar to an RKL install.  If you fail to do this, you'll get a "Loading Monochrome" screen an it'll go no further.  
![CertsFigure1.jpeg](/img/user/Assets/Images/CertsFigure1.jpeg)



---

---
## Detailed Walkthrough (work in progress)


### Step 1 - Preparation 
1. Before beginning, find a dispenser side that is working (likely the opposite side of the dispenser you’re working on), swipe your blue maintenance card, select “Retrieve System Information” (1), and “Print System Information” (2).
	1. If you hear a grinding sound, the printer is jammed.  Either fix it or perform this process on another dispenser.
	2. Once you get the print out, save it.  We’ll need it later. 


### Step 2 - Physical Replacement
1. Unplug dispenser
2. Unplug all cables on UPM
	1. If you are unfamiliar with where these cables go, you may want to take a picture before you remove any cables
3. Remove UPM
	1. You need a T20 torx bit to remove the metal retainer holding the UPM in place
	2. It will likely be stuck in place.  Put firm pressure on the button side of the UPM and it will come off.  
4. Put the UPM face down beside the replacement UPM (also face down) and take a picture.  You will need the serial number (8 digit number) on both for paperwork. (I like to put the old one on the left).
	1. ![UPMBacks.jpg](/img/user/Assets/Images/UPMBacks.jpg)
5. Perform the same steps backward to install the new UPM.  
6. Before powering on the dispenser, unplug the 2-wire and replace it with a jumper
	1. We want to avoid the unprogrammed UPM from taking down other dispensers while we work in it.  


### Step 3 - Activating the UPM
1. Plug in the dispenser and take a picture of the very first screen shown.  It has the serial number of the UPM and we need it to access the programming screen.  
2. Watch the bottom left hand corner till you see “<1> Enter Setup” and press 1.  
3. Enter the last 6 digits of the serial number you took a picture of
4. Time to activate the UPM!  Select “<8> - Secure Menu”
5. Open your Gilbarco activation software to input the info on the screen. (Steps to how to use the activation software will be HERE)
6. Once you receive a text with the activation code, input that into the black box
7. Once you’re in, select “<3> - System Activation”
8. Next, select “<1> - Unit Activation”
9. All three components should now say Enabled
10. At this point, instructions change depending on if you have an OMNIA or an SSOM


### Step 3a - if you have an OMNIA
1. Do things


### Step 3b - if you have an SSOM
1. In the Secure Menu, select “<2> - Network Menu”
2. Get out that printout from our preparation 
	1. Find the heading “Network Configuration”
	2. The IP address is made up of 4 numbers separated by dots.  Note the first three.  The last number should be 1 for A side and 3 for B side.  
	3. Make sure that the first three numbers are correct for the IP address (it usually is)
	4. Next, do the same for the Subnet Mask (it’s usually wrong).
	5. Finally, check the gateway.  It will almost definitely be wrong.  
	6. Select ok and it will ask you to press the button on the back of the card reader.  Do so.  
	7. Once it’s done, you can select ok.  It may ask you to assign up addresses to the GSOM, but you can hit cancel to exit as it was already setup.
	8. 


### Step 4 - Programming the UPM

Use the [[Flexpay IV CRIND.pdf]] quick reference guide.  It is located in the [[Guides, References, and Troubleshooting/Misc/REF - Manuals and Guides\|REF - Manuals and Guides]] note.

### Step 5 - Updating Software and Installing RKLs and Certs

** Before continuing, be aware that many big brands are picky about how they want the following steps done.  Check and make sure there is no playbook for your brand for UPMs and whitelisting (Circle K in particular has a procedure they want followed [[CircleK-UPM-Replacement.pdf]] ) ** 

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

