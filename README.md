# Enterprise Network Design using Cisco Packet Tracer
- A Cisco Packet Tracer project that simulates a small enterprise network with redundant gateway architecture, dynamic routing, centralized network services, and secure device management.
- The project demonstrates common enterprise networking concepts based on Cisco technologies and CCNA-level fundamentals.

# Project Objectives
This project was developed to simulate a real world enterprise network environment and practice configuring Cisco networking technologies, including:
- Department-based VLAN segmentation
- Inter-VLAN communication
- Gateway redundancy
- Dynamic routing
- Centralized network services
- Secure remote administration
- Basic Layer 2 security
- etc ....

# Features
## Layer 2
- VLAN Configuration
- Access Port Configuration
- IEEE 802.1Q Trunking
- Port Security (Sticky MAC)
- SSH

## Layer 3
- Layer 3 Switching
- Inter-VLAN Routing
- HSRP (Hot Standby Router Protocol)
- OSPF Dynamic Routing
- WAN Connectivity

## Network Services
- HTTP
- DHCP
- DHCP Relay
- DNS Server
- Web Server

## Security
- SSH Version 2
- Local User Authentication
- Disabled Telnet
- Password Encryption
- Port Security

# Network Architecture
The enterprise network consists of two sites connected through a WAN link.
- Headquarters (HQ)
- Branch Office

Each site contains:
- Layer 3 Core Switches
- Access Switches
- Department VLANs
- End Devices

Gateway redundancy is implemented using HSRP while routing between sites is handled by OSPF:

# Validation & Testing
The following functionalities were successfully tested.
- VLAN Communication
- Inter-VLAN Routing
- HSRP Failover
- OSPF Neighbor Adjacency
- DHCP Address Assignment
- DNS Resolution
- HTTP Connectivity
- SSH Remote Login
- Port Security

Screenshots are available in the **screenshots/** directory.

# Future Improvements
Possible enhancements for future versions:
- SNMP Monitoring
- Expand the network
- Syslog Server
- NTP
- IPv6 Support
- EtherChannel
- ACL Policies
- Network Management VLAN

