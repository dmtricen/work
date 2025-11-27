---
{"dg-publish":true,"permalink":"/guides-references-and-troubleshooting/verifone/commander/trbl-troubleshooting-verifone-pos-issues/"}
---


- ### Situation 1
	- Every time the customer prepays for gas, once they are finished, the sale comes back asking for the money again.
		- The Commander can't communicate with the DCR.  That's the only way it knows when things are finished and how much was pumped.  Go and make sure there are no errors on the screen out at the dispenser.
- ### Situation 2
	- There is an error on screen about Onboarding not being done.  
		- A requirement of having a new Commander installed is to have it onboarded.  The owner must go to the website and create a username and password.  Then, sign into the the C-Store config and go to On boarding and put in their credentials.  It's only good for about a month, it will give a message, then it will behave forever more.  