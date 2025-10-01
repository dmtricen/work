---
{"dg-publish":true,"permalink":"/troubleshooting/leak-detection/veeder-root/veeder-root-tls/","tags":["Keep/Color/Purple","Keep/Label/Troubleshooting-Guide"]}
---

[[Veeder-Root TLS3XX.pdf]]
[[Veeder-Root TLS-450+.pdf]]


***TLS-3xx***

#### **How to configure TCP-IP card**

**Establish an address to telnet**
- Select an ip address unused but on your subnet
- Open admin command prompt
- arp -s (ip address) (MAC address with dashes)
- arp -a (verify entry exists)

 **Telnet into TLS**
- telnet (ip address) 9999
- Hit enter immediately to get menu
- Verify ip address and port

————————————————————————

**PLLD Controller Module**

![PLLD Controller Module1.jpeg](/img/user/Assets/Images/PLLD%20Controller%20Module1.jpeg)

![PLLD Controller Module2.jpeg](/img/user/Assets/Images/PLLD%20Controller%20Module2.jpeg)