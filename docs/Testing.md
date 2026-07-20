# Network Testing
This document records the validation of all implemented network functions.

# Test 1 - VLAN Connectivity
Objective
Verify communication between hosts in the same VLAN.
Result
PASS

# Test 2 - Inter-VLAN Routing
Objective
Verify routing between different VLANs.
Result
PASS

# Test 3 - HSRP
Objective
Shutdown the active multilayer switch and verify that the standby switch becomes active.
Expected Result
Gateway remains reachable.
Result
PASS

# Test 4 - OSPF
Objective
Verify OSPF neighbor adjacency.
Command
show ip ospf neighbor
Result
PASS

# Test 5 - DHCP
Objective
Verify automatic IP assignment.
Command
ipconfig
Result
PASS

# Test 6 - DNS
Objective
Verify hostname resolution.
Command
ping www.company.local
Result
PASS

# Test 7 - Web Server
Objective
Access the internal website.
Result
PASS

# Test 8 - SSH
Objective
Verify remote login to network devices.
Command
ssh -l admin 192.168.x.x
Result
PASS

# Test 9 - Port Security
Objective
Connect an unauthorized device to a secured access port.
Expected Result
Traffic is blocked.
Result
PASS
