# Project-Small-Office-Network-Design
Enterprise Network Project in Cisco Packet Tracer  —  Small Office Network Design &amp; Implementation


Project: Small Office Network Design
====================================

Scenario

A startup company has 3 departments: Administration, Sales, and IT. The office has around 30 employees. You need to design a network that connects all users, allows them to share resources (like a file server and printer), and provides internet access.


Requirements
------------
3 VLANs

	VLAN 10 → Administration (10 users)
	VLAN 20 → Sales          (15 users)
	VLAN 30 → IT             (5 users)


IP Addressing
-------------
Use a private Class C network 192.168.1.0/24.

	VLAN 10 (Admin): 192.168.1.0/27 → GW 192.168.1.1
	VLAN 20 (Sales): 192.168.1.32/27 → GW 192.168.1.33
	VLAN 30 (IT): 192.168.1.64/27 → GW 192.168.1.65

Server: 192.168.1.100 (File/Print server)

Internet router WAN: DHCP from ISP

Inter-VLAN communication
A router-on-a-stick (one router connected to the switch via trunk) provides inter-VLAN routing.

DHCP
Configure DHCP pools on the router so PCs automatically get IP addresses.


Deliverables
------------

Network diagram
VLAN configuration
IP addressing table
DHCP configuration
Testing (ping across VLANs and to the internet)

Topology (Logical)
------------------

1 Router (for Inter-VLAN routing + NAT)
1 Switch (supports VLAN + trunk)
3 PCs (representing each department, you can add more in Packet Tracer)
1 Server (File/Print)


<img width="1424" height="777" alt="Project Small Office Network Diagram" src="https://github.com/user-attachments/assets/3ec5971c-7719-4e75-9918-a29b7368c06f" />
