<h1> LAN-Documentation-and-Switch-Configuration </h1>


---
Hello everyone, in this lab I created a simple Local Area Network (LAN) network that uses Router On a Stick"(ROAS). Hopefully you all find this lab insightful!

<h2>Table of Contents</h2> 

- Step 1 – Network Topology Setup
- Step 2 – Basic Switch Configuration
- Step 3 – VLAN Assignment to Ports
- Step 4 – Switch to Router Port Configuration (Trunking)
- Step 5 – Router Subinterface Configuration (ROAS)
- Step 6 – Assigning Static IPs to PCs
- Step 7 – Connectivity Testing
- Summary/Take Aways


<h3>Technology Utilized</h3>
- Packet Tracer (or any other simulation tool like EVE-NG or GNS3)

I used Packet Tracer for simplicity—and because it's free.

---
<h2>Step 1 – Network Topology Setup</h2>
This step focues on getting all of the networking, end devices and media needed.
Which in this case it is:
- 4 PCs
- 2 2960 Switches
- 1 2901 Router

![image alt](https://github.com/GerardoSierra-IT/LAN-Documentation-and-Switch-Configuration/blob/8570563d5ebda850c463f4b8ef4514a0a9276d47/LAN%20before%20it%20was%20all%20up.jpg)

---
<h2>Step 2 – Basic Switch Configuration</h2>
In this step  we begin basic configuration such as hostname, creating the 2 vlans and . Other than the hostname, both switches should be configured this same here.

![image alt](https://github.com/GerardoSierra-IT/LAN-Documentation-and-Switch-Configuration/blob/501f17ffe725f18158f2ccfe4bbb135abcf0894b/Switch%20configurations.jpg)

---
<h2>Step 3 – VLAN Assignment to Ports</h2>
Next, we move into a 2 part step. Where we configure each port their designated vlan. This essentially assigns the role/ purpose for that port. Similar to the previous step, make sure that both switches have the same configurations. As we wouldnt want to run into any issues because one switch knows of a vlan but is unkown to the other switch.

The second part to this step involves configuring the ports used to connect with the other switch (In my case it is port Fastethernet0/24 on SW1 and port Fastethernet0/24 on SW2)


![image alt](https://github.com/GerardoSierra-IT/LAN-Documentation-and-Switch-Configuration/blob/b5685843d71be0b0bf13e8a3eae384267d1b9fac/trunk%20configurations.jpg)


---
<h2>Step 4 – Switch to Router Port Configuration (Trunking)</h2>
This step then continues the process of assigning the role / purpose of in this case port Fastethernet 0/5 (this is my connection to my router). To allowing both vlan 10 and 20.

![image alt](https://github.com/GerardoSierra-IT/LAN-Documentation-and-Switch-Configuration/blob/b5685843d71be0b0bf13e8a3eae384267d1b9fac/forgotten%20configurations%20for%20SW1.jpg)


---
<h2>Step 5 - Router Subinterface Configuration (ROAS)</h2>
This step invloves configurations done on the router. Where we allow different devices on different vlans to be able to communicate with each other.

![image alt](https://github.com/GerardoSierra-IT/LAN-Documentation-and-Switch-Configuration/blob/b5685843d71be0b0bf13e8a3eae384267d1b9fac/router%20configurations.jpg)

---
<h2>Step 6 - Assigning Static IPs to PCs</h2>
Here we assign a static IP address to each PC. You can use any private IP address for this, in this lab I used the 192.168.0.0
Assign a static IP address to each PC. You can use any private IP range, but for this lab I used:

VLAN 10:

PC1: 192.168.10.10/24

PC2: 192.168.10.11/24

VLAN 20:

PC3: 192.168.20.10/24

PC4: 192.168.20.11/24

PC > Desktop > IP Configuration


![image alt](https://github.com/GerardoSierra-IT/LAN-Documentation-and-Switch-Configuration/blob/fb53b3a2e7982a11b747ddfeb447bcd106765953/pc%20step1.jpg)
![image alt](https://github.com/GerardoSierra-IT/LAN-Documentation-and-Switch-Configuration/blob/fb53b3a2e7982a11b747ddfeb447bcd106765953/pc%20step%202.jpg)

---
<h2>Step 7 – Connectivity Testing</h2>

PC > Desktop > Command Prompt

![image alt](https://github.com/GerardoSierra-IT/LAN-Documentation-and-Switch-Configuration/blob/29fca487f205bdb180c38c64fc1acacf449fe23f/successful%20pings.jpg)
---

<h2> Summary/ Take Away </h2>

<h4>We successfully created a small but effective LAN that allows end devices across different VLANs to communicate using a router-on-a-stick configuration. This kind of setup is common in enterprise environments for network segmentation and security. </h4> 
---
