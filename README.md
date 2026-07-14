# Campus Network Infrastructure - GNS3

> A Cisco GNS3-based campus network infrastructure implementing VLAN segmentation, Router-on-a-Stick, Inter-VLAN Routing, DHCP, SSH, and Port Security.

---

## 📖 Project Overview

This project demonstrates the design and implementation of a hierarchical campus network using Cisco IOS devices in GNS3.

The network was developed as part of my self-learning journey to strengthen my practical networking skills while preparing for Cisco CCNA.

The implementation includes VLAN segmentation, secure switch management, inter-VLAN routing, centralized DHCP services, and port security.

---

## 🏗 Network Topology



```
ScreenShots\Topology.png
```

---

## 🎯 Project Objectives

- Design a hierarchical campus network
- Implement VLAN segmentation
- Configure Router-on-a-Stick
- Enable Inter-VLAN Routing
- Configure DHCP for all VLANs
- Secure remote device management using SSH
- Implement Port Security using Sticky MAC
- Build a scalable network structure

---

# 🏛 Network Architecture

```
                 R-GATEWAY
                     │
               Router-on-a-Stick
                     │
                 SW-CORE
                     │
        ┌────────────┴────────────┐
        │                         │
    SW-DIST1                 SW-DIST2
   ┌───┼────┐               ┌───┼────┐
 SW-CEE SW-EIE SW-LIB    SW-MENA SW-MME SW-IDS
```

Architecture Model

- Core Layer
- Distribution Layer
- Access Layer

---

# 🌐 VLAN Plan

| VLAN | Department | Gateway |
|------|------------|------------|
|10|Civil and Environmental Engineering|192.168.10.1|
|20|Electrical and Information Engineering|192.168.20.1|
|30|Marine Engineering and Naval Architecture|192.168.30.1|
|40|Mechanical and Manufacturing Engineering|192.168.40.1|
|50|Department of Interdisciplinary Studies|192.168.50.1|
|60|Central Library|192.168.60.1|
|99|Management VLAN|192.168.99.1|
|100|Native VLAN|Unused|

---

# 📡 IP Addressing Scheme

| Network | Subnet |
|----------|----------------|
|VLAN 10|192.168.10.0/24|
|VLAN 20|192.168.20.0/24|
|VLAN 30|192.168.30.0/24|
|VLAN 40|192.168.40.0/24|
|VLAN 50|192.168.50.0/24|
|VLAN 60|192.168.60.0/24|
|Management VLAN|192.168.99.0/24|

---

# ⚙ Technologies Used

- Cisco IOS
- Cisco GNS3
- VLAN (802.1Q)
- Router-on-a-Stick
- Inter-VLAN Routing
- DHCP
- SSH
- Port Security
- Sticky MAC
- Hierarchical Network Design

---

# 🔐 Security Features

✔ SSH Version 2

✔ Local User Authentication

✔ Port Security

✔ Sticky MAC Address Learning

✔ Management VLAN

✔ Native VLAN Separation

---

# 📋 Device List

| Device | Quantity |
|----------|---------|
|Router|1|
|Core Switch|1|
|Distribution Switches|2|
|Access Switches|6|
|VPCS Clients|12|

---

# ✅ Project Verification

The following features were successfully tested.

- VLAN Communication
- Inter-VLAN Routing
- DHCP Address Assignment
- SSH Remote Login
- Port Security Sticky MAC
- Trunk Configuration
- Router-on-a-Stick
- End-to-End Connectivity

---

# 📷 Screenshots

### Network Topology

*(Insert topology image)*

---

### Router-on-a-Stick

*(Insert screenshot)*

---

### DHCP Bindings

*(Insert screenshot)*

---

### SSH Configuration

*(Insert screenshot)*

---

### Port Security

*(Insert screenshot)*

---

### Inter-VLAN Routing Test

*(Insert screenshot)*

---

# 📂 Repository Structure

```
Campus-Network-Infrastructure-GNS3
│
├── README.md
├── LICENSE
│
├── topology
│   └── campus_network_topology.png
│
├── configs
│   ├── R-GATEWAY.txt
│   ├── SW-CORE.txt
│   ├── SW-DIST1.txt
│   ├── SW-DIST2.txt
│   ├── SW-CEE.txt
│   ├── SW-EIE.txt
│   ├── SW-LIB.txt
│   ├── SW-MENA.txt
│   ├── SW-MME.txt
│   └── SW-IDS.txt
│
└── screenshots
    ├── topology.png
    ├── inter-vlan-routing.png
    ├── dhcp.png
    ├── ssh.png
    ├── port-security.png
```

---

# 🚀 Future Improvements

- Dynamic Routing (OSPF)
- HSRP
- SNMP Monitoring
- Syslog Server
- Network Automation using Python
- Netmiko
- Ansible
- Zabbix Monitoring
- pfSense Integration

---

# 👨‍💻 Author

**Asitha Pathirathna**

Faculty of Engineering

Cisco CCNA Student

Network Engineering Enthusiast

---

# 📄 License

This project is released under the MIT License.

---

## ⭐ If you found this project useful, consider giving it a star.