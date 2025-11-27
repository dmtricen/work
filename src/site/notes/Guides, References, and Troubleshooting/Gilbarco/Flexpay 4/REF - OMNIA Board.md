---
{"dg-publish":true,"permalink":"/guides-references-and-troubleshooting/gilbarco/flexpay-4/ref-omnia-board/"}
---

![Omnia1.jpg](/img/user/Assets/Images/Omnia1.jpg)

Software update:
- There are two different software packages in the extranet that could be used for the Omnia, the standard package and the “Encore Experience”.  Call TAC to determine which should be installed at the site (we can’t tell the difference).  
- Also note there is a package called ICS.  No idea what it does.  Ask TAC if it needs installation.  
- When dropping software into the software updater, drop in the zipped version, not the extracted.  



---

## Troubleshooting

#### No communication in an Passport (MOC) environment

If you are using an OMNIA in an MOC environment, you have to program the OMNIA to use MOC instead of Generic CRIND.  If you do that, an led will light up on the right side of the board labeled "MOC".  If that light isn't lit, the board might be accessible on the network, but it won't pass information to the PCN correctly and you'll likely get an error 50.  