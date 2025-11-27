---
{"dg-publish":true,"permalink":"/guides-references-and-troubleshooting/verifone/commander/guid-oemv-upgrade-steps/"}
---

1) Call Cybera and request
	1) OEMV configuration 
	2) New Port Map
2) Setup C18 and upgrade (switch 1) and sync
3) Modify peripherals ports
4) Pinpad Setup
	1) physically install
	2) Call (Exxon or bypass) 
		1) Provide vend id or address
		2) Ask what debit card encryption is needed
5) Update DCR Config in Commander

![OEMVupgrade1.jpeg](/img/user/Assets/Images/OEMVupgrade1.jpeg)
		1) Ensure “Enable Debit”, NCF Mode = EMV enabled, and IP is 10.5.55.* (71 and on) for each dcr

6) PDL Downloads![OEMVupgrade2.jpeg](/img/user/Assets/Images/OEMVupgrade2.jpeg)
7) Ensure UPMs are programmed and homeplugs installed


1 - Nic A
9-16 - Verifone Zone
2-4 - Back OPs
7 - EMV (Gilbarco)
8 - Applause Media

*Note* C18 printer in port 4 ONLY



