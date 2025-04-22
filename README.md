# LAN-Documentation-and-Switch-Configuration


---
Hello everyone, in this lab I created a simple Local Area Network (LAN) network that uses Router On a Stick"(ROAS). Hopefully you all find this lab insightful!

# Table of Contents

- [Step 1](#step-8-mock-meeting-post-initial-discovery-scan-server-team)
- [Step 2](#step-9-mock-cab-meeting-implementing-remediations)
- [Step 3](#remediation-round-1-outdated-wireshark-removal)
- [Step 4](#remediation-round-2-insecure-protocols--ciphers)
- [Step 5](#remediation-round-3-guest-account-group-membership)
- [Step 6](#remediation-round-4-windows-os-updates)
- [Step 7](#f)
- [Step 8](#f)
- [Summary/Take Aways](#first-cycle-remediation-effort-summary)


# Technology Utilized
- Packet Tracer or any other simulation tool EVE-NG or GNS3 (I just went with Packet Tracer for simplicity and it's free)

---

This step focues on getting all of the networking, end devices and media needed.
Which in this case it is:
- 4 PCs
- 2 2960 Switches
- 1 2901 Router
![image alt](https://github.com/GerardoSierra-IT/LAN-Documentation-and-Switch-Configuration/blob/8570563d5ebda850c463f4b8ef4514a0a9276d47/LAN%20before%20it%20was%20all%20up.jpg)

---
In this step  we begin basic configuration such as hostname, creating the 2 vlans and . Other than the hostname, both switches should be configured this same here.

![image alt](https://github.com/GerardoSierra-IT/LAN-Documentation-and-Switch-Configuration/blob/501f17ffe725f18158f2ccfe4bbb135abcf0894b/Switch%20configurations.jpg)

---
Next, we configure each port their designated vlan. This essentially assigns the role/ purpose for that port. Similar to the previous step, make sure that both switches have the same configurations. As we wouldnt want to run into any issues because one switch knows of a vlan but is unkown to the other switch.

![image alt](https://github.com/GerardoSierra-IT/LAN-Documentation-and-Switch-Configuration/blob/b5685843d71be0b0bf13e8a3eae384267d1b9fac/configuring%20vlans%20on%20ports.jpg)

---
This step then continues the process of assigning the role / purpose of in this case port Fast ethernet 0/5. To allowing both vlan 10 and 20. Remeber to do this on the other switch as well.

![image alt](https://github.com/GerardoSierra-IT/LAN-Documentation-and-Switch-Configuration/blob/b5685843d71be0b0bf13e8a3eae384267d1b9fac/forgotten%20configurations%20for%20SW1.jpg)

---

![image alt](https://github.com/GerardoSierra-IT/LAN-Documentation-and-Switch-Configuration/blob/b5685843d71be0b0bf13e8a3eae384267d1b9fac/router%20configurations.jpg)

---
This 
![image alt](https://github.com/GerardoSierra-IT/LAN-Documentation-and-Switch-Configuration/blob/b5685843d71be0b0bf13e8a3eae384267d1b9fac/trunk%20configurations.jpg)

---



---

![image alt]()

---
Summary/ Take Away


---
