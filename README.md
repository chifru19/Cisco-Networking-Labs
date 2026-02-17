# Cisco-Networking-Labs
A portfolio of Cisco Packet Tracer labs and Python scripts demonstrating expertise in secure network design, VLAN segmentation, and infrastructure automation."
# Project 1: Secure SOHO Network Implementation
![Networking](https://img.shields.io/badge/Skill-Networking-blue) 
![Security](https://img.shields.io/badge/Skill-Security+-green)
![Status](https://img.shields.io/badge/Status-Completed-success)

## 🎯 Project Objective
The goal of this project was to design and implement a secure Small Office/Home Office (SOHO) network that integrates both wired and wireless infrastructure. This lab simulates a real-world startup environment requiring centralized IP management and hardened wireless security.

## 🏗️ Network Topology
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/7f5e4c13-5338-4d9b-b217-79760e35879a" />


### Components Used:
* **Router:** Generic Wireless Router (WRT300N)
* **Switching:** Integrated 4-port Ethernet switch
* **End Devices:** 2x Desktop PCs (Wired), 1x Laptop (Wireless), 1x Network Printer

## ⚙️ Configuration Details
* **Layer 3 (Network):** Implemented **DHCP** for automated IPv4 addressing (`192.168.0.0/24`).
* **Wireless Security:** Configured **WPA2-AES (Personal)** encryption to secure the `Tesla_Lab` SSID.
* **Hardware Integration:** Upgraded Laptop hardware with a **WPC300N Wireless Interface Card** to support 802.11n standards.

## ✅ Verification & Results
To ensure the "Physical" and "Logical" layers were correctly established, the following tests were performed:
1. **Connectivity Test:** Successful ICMP `ping` from Laptop0 (Wireless) to Printer0 (Wired).
2. **Security Audit:** Verified that unauthorized devices cannot join the SSID without the WPA2-AES handshake.
3. **Addressing:** Confirmed all devices correctly leased IP addresses from the DHCP pool.
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/6ea85c52-1cf5-490a-b4b9-c7eae103591e" />

--- 
Project 2: Enterprise VLAN Segmentation
Objective: Implement Layer 2 security by isolating departments into separate Virtual LANs (VLANs) to minimize the attack surface and manage broadcast traffic.

🛠️ Technical Implementation
VLAN Configuration: Created VLAN 10 (HR) and VLAN 20 (Sales) on a Cisco Catalyst Switch.

Access Port Assignment:

Ports Fa0/1 - Fa0/2 assigned to VLAN 10.

Ports Fa0/3 - Fa0/4 assigned to VLAN 20.

IP Schema: Utilized distinct subnets (192.168.10.x and 192.168.20.x) to align with VLAN boundaries.

🧪 Verification & Testing
Intra-VLAN Connectivity: Verified successful ICMP pings between hosts within the same VLAN.

VLAN Isolation: Confirmed that traffic between VLAN 10 and VLAN 20 is blocked at Layer 2, ensuring department data privacy.
*Created by [Frank Fru] as part of the Network Infrastructure Portfolio.*
