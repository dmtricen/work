---
{"dg-publish":true,"permalink":"/guides-references-and-troubleshooting/gilbarco/flexpay-4/ref-dcm-2-and-ssom/"}
---

*A pdf related to this entry is available.  Refer to [[Guides, References, and Troubleshooting/Misc/REF - Manuals and Guides\|REF - Manuals and Guides]] for a link.*

[[SSOM and DCM2.pdf]]

![DCM2-1.jpg](/img/user/Assets/Images/DCM2-1.jpg)

Above is a DCM 2.2.  It is made up of a CCP board with 2 GSOM attached and an SSOM (attached to the back of the board between it and the back plate).  This functions as the CRIND logic board.  

---
### CCP Board

![DCM2-2.jpeg](/img/user/Assets/Images/DCM2-2.jpeg)


---
### GSOM

![DCM2-3.jpeg](/img/user/Assets/Images/DCM2-3.jpeg)


---
### SSOM

![DCM2-4.jpeg](/img/user/Assets/Images/DCM2-4.jpeg)

The SSOM turns the CCP into an IP router.  
At a site with a standard IP scheme, each UPM 10.5.55.7x (replace x with the dispenser number).  When you have a CCP without an SSOM, you would setup your IPs like this

- Dispenser 1 UPM side A - 10.5.55.71
- Dispenser 1 Card Reader side A - 10.5.55.72
- Dispenser 1 UPM side B - 10.5.55.73
- Dispenser 1 Card Reader side B - 10.5.55.74
- Dispenser 2 UPM side A - 10.5.55.81
- Dispenser 2 Card Reader side A - 10.5.55.82
- Dispenser 2 UPM side B - 10.5.55.83
- Dispenser 2 Card Reader side B - 10.5.55.84

And so on.  This is needed because we don't have a router to insulate the IP addresses.  If you have an SSOM, the addresses on the dispenser will look more like the addresses you'd use on an OMNIA.  

- Dispenser 1 UPM side A - 172.16.100.1
- Dispenser 1 Card Reader side A - 172.16.100.2
- Dispenser 1 UPM side B - 172.16.100.3
- Dispenser 1 Card Reader side B - 172.16.100.4
- Dispenser 2 UPM side A - 172.16.100.1
- Dispenser 2 Card Reader side A - 172.16.100.2
- Dispenser 2 UPM side B - 172.16.100.3
- Dispenser 2 Card Reader side B - 172.16.100.4

You would then connect to the SSOM and make the IP address of side A 10.5.55.71 and side B 10.5.55.72.  

---


Make sure your jumpers are set correctly.  Smart crind and VLAN should be off.  

Updating the SSOM may require migration to upgrade fully.  
1. Download the update and the migration tool from extranet.  
2. Load the migration software zip file on a usb drive (not the extracted) and place it in the dcm2 then turn on power.  
3. Connect to the old SSOM and perform a software upgrade and select the zip file.  
4. Once it’s done (it takes a while) pull the usb out. 
5. Once it reboots, sign in again and run the software upgrade and select the upgrade zip (unextracted) from your pc.  This takes a LONG time to be patient.  

NOTE - Brandon refers to this board as the “CCP” board.  No idea what that stands for.  

