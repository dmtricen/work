---
{"dg-publish":true,"permalink":"/troubleshooting/dispenser-troubleshooting/gilbarco/flexpay-iv/dcm-2-and-ssom/"}
---

*A pdf related to this entry is available.  Refer to [[Troubleshooting/Manuals and Guides\|Manuals and Guides]] for a link.*

[[SSOM and DCM2.pdf]]

![DCM2-1.jpg](/img/user/Assets/Images/DCM2-1.jpg)

Above is a DCM 2.2.  It is made up of a CCP board with 2 GSOM attached and an SSOM (attached to the back of the board between it and the back plate).  This functions as the CRIND logic board.  

---
CCP Board

![DCM2-2.jpeg](/img/user/Assets/Images/DCM2-2.jpeg)


---
GSOM

![DCM2-3.jpeg](/img/user/Assets/Images/DCM2-3.jpeg)


---
SSOM

![DCM2-4.jpeg](/img/user/Assets/Images/DCM2-4.jpeg)


---


Make sure your jumpers are set correctly.  Smart crind and VLAN should be off.  

Updating the SSOM may require migration to upgrade fully.  
1. Download the update and the migration tool from extranet.  
2. Load the migration software zip file on a usb drive (not the extracted) and place it in the dcm2 then turn on power.  
3. Connect to the old SSOM and perform a software upgrade and select the zip file.  
4. Once it’s done (it takes a while) pull the usb out. 
5. Once it reboots, sign in again and run the software upgrade and select the upgrade zip (unextracted) from your pc.  This takes a LONG time to be patient.  

NOTE - Brandon refers to this board as the “CCP” board.  No idea what that stands for.  

