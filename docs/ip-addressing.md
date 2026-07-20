# VLAN Addressing

| VLAN | Name | Network | Gateway (HSRP VIP) |
|------|------|--------|---------|
| 10 | HQ-HR | 192.168.10.0/24 | 192.168.10.1 |
| 20 | HQ-SALES | 192.168.20.0/24 | 192.168.20.1 |
| 30 | HQ-FINANCE | 192.168.30.0/24 | 192.168.30.1 |
| 40 | BR-HR | 192.168.40.0/24 | 192.168.40.1 |
| 50 | BR-SALES | 192.168.50.0/24 | 192.168.50.1 |
| 60 | BR-FINANCE | 192.168.60.0/24 | 192.168.60.1 |
| 100 | Server | 192.168.100.2/24 | 192.168.60.1 |

# Infrastructure IP Addressing

| Device | Interface | IP Address |
|------|--------|---------|
| HQ-MLS1 | Vlan10 | 192.168.10.2 |
| HQ-MLS2 | Vlan10 | 192.168.10.3 |
| HQ-MLS1 | Vlan20 | 192.168.20.2 |
| HQ-MLS2 | Vlan20 | 192.168.20.3 |
| HQ-MLS1 | Vlan30 | 192.168.30.2 |
| HQ-MLS2 | Vlan30 | 192.168.30.3 |
| BR-MLS1 | Vlan40 | 192.168.40.2 |
| BR-MLS2 | Vlan40 | 192.168.40.3 |
| BR-MLS1 | Vlan50 | 192.168.50.2 |
| BR-MLS2 | Vlan50 | 192.168.50.3 |
| BR-MLS1 | Vlan60 | 192.168.60.2 |
| BR-MLS2 | Vlan60 | 192.168.60.3 |

# Wan Addressing

| Device | Interface | IP Address |
|------|--------|---------|
| HQ-R1 | Serial0/0/0 | 10.10.10.1/30 |
| BR-R1 | Serial0/0/0 | 10.10.10.2/30 |

# Server

| Server | IP | Other |
|------|--------|---------|
| DHCP Server | 192.168.100.0/24 | |
| DNS Server | 192.168.100.10/24 | testing.com |





