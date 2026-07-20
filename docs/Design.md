# Network Design
## Overview
This project simulates a small enterprise network consisting of two sites:
- Headquarters (HQ)
- Branch Office

Both sites are connected through a WAN link and use dynamic routing to exchange routing information.

# Design Goals
The network was designed with the following objectives:
- Improve network segmentation using VLANs.
- Provide high availability using HSRP.
- Support dynamic routing with OSPF.
- Deploy centralized network services.
- Secure remote administration using SSH.
- Implement Layer 2 security using Port Security.

# VLAN Design
-Vlan10 : 192.168.10.2 : HQ-HR
-Vlan20 : 192.168.20.2 : HQ-SALES
-Vlan30 : 192.168.30.2 : HQ-FINANCE
-Vlan40 : 192.168.40.2 : BR-HR
-Vlan50 : 192.168.50.2 : BR-SALES
-Vlan60 : 192.168.60.2 : BR-FINANCE

# Layer 2 Design
-Each department is placed in its own VLAN to reduce broadcast traffic and improve security.
-802.1Q trunk links are used between access switches and multilayer switches.

# Layer 3 Design
-Inter-VLAN routing is implemented using Switch Virtual Interfaces (SVIs) on multilayer switches.
-OSPF is used as the dynamic routing protocol between the Headquarters and Branch sites.

# High Availability
HSRP provides gateway redundancy.
Each VLAN has:
- Virtual Gateway
- Active MLS
- Standby MLS

If the active multilayer switch fails, the standby switch automatically becomes the active gateway.

# Network Services
The enterprise network provides:
- DHCP
- DHCP Relay
- DNS
- Web Server

These services allow hosts to obtain IP addresses automatically and access internal resources.

# Security
Implemented security features include:
- SSH Version 2
- Local user authentication
- Encrypted passwords
- Disabled Telnet
- Port Security using Sticky MAC

# Routing
-OSPF Area 0 is used throughout the network.
-Dynamic routing automatically exchanges routes between the two sites.

