# Cisco-Networking-Labs
A portfolio of Cisco Packet Tracer labs and Python scripts demonstrating expertise in secure network design, VLAN segmentation, and infrastructure automation."
# Project 1: Secure SOHO Network Implementation
![Networking](https://img.shields.io/badge/Skill-Networking-blue) 
![Security](https://img.shields.io/badge/Skill-Security+-green)
![Status](https://img.shields.io/badge/Status-Completed-success)

## 🎯 Project Objective
The goal of this project was to design and implement a secure Small Office/Home Office (SOHO) network that integrates both wired and wireless infrastructure. This lab simulates a real-world startup environment requiring centralized IP management and hardened wireless security.

## 🏗️ Network Topology
> [!TIP]
> **Insert your Packet Tracer Workspace Screenshot Here**
> (Drag and drop your image file into this line in GitHub to upload it)

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

---
*Created by [Your Name] as part of the Network Infrastructure Portfolio.*
