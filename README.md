# SOHO Network Design and Implementation using VLANs

## 📌 Project Overview
This project demonstrates the **design and implementation of a Small Office Home Office (SOHO) network** for a newly established company branch.  
The network is designed to operate independently from the headquarters (HQ) and supports **three departments**, each isolated using **VLANs**, while still allowing **inter-VLAN communication**.

The implementation focuses on **VLAN segmentation, subnetting, DHCP configuration, wireless access points, and inter-VLAN routing** using Cisco networking devices.

---

## 🏢 Network Requirements
- One **Cisco Router** and one **Cisco Switch**
- Three departments:
  - Admin / IT
  - Finance / HR
  - Customer Service / Reception
- Separate **VLAN** for each department
- Separate **wireless network (SSID)** for each department
- Automatic IPv4 address allocation using **DHCP**
- Full communication between departments using **Inter-VLAN Routing**
- Base network provided by ISP: `192.168.1.0`

---

## 🛠 Tools & Technologies
- Cisco Packet Tracer
- Cisco Router and Switch
- VLAN Configuration
- Subnetting
- DHCP Server
- Wireless Access Points
- Inter-VLAN Routing (Router-on-a-Stick)

---

## 🧩 Network Design Highlights
- VLAN-based logical separation for security and traffic isolation
- Subnetting to efficiently allocate IP addresses
- Trunk links between router and switch
- Router sub-interfaces acting as default gateways for VLANs
- DHCP pools for each VLAN
- Wireless access points mapped to respective VLANs

---

## ⚙️ Implementation Summary
### VLAN Configuration
```bash
switchport mode access
switchport access vlan <vlan_id>
