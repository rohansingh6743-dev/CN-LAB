Assignment 2: Packet Flow Visualization Using Simulation Mode

Experiment Objectives
Students will use Packet Tracer Simulation Mode to observe how packets move between devices, how switches learn MAC addresses, and how ICMP echo request/reply travels through a small network.

Components required : 
Hardware Components (in Cisco Packet Tracer):
•	1 Switch (2960) 
•	3 PC
•	Copper Straight Through cables 


Packet Flow in a Network
When a device sends data to another device, the data is divided into small units called packets. These packets travel through network devices such as switches and routers to reach the destination.

 ICMP (Internet Control Message Protocol)
ICMP is used for sending error messages and operational information.
The most common use is the ping command, which checks connectivity between devices.
•	ICMP Echo Request → Sent by source device 
•	ICMP Echo Reply → Sent by destination device 

 ARP (Address Resolution Protocol)
ARP is used to map an IP address to a MAC address.
 Before sending data:
•	Source device must know the destination MAC address 
•	If unknown, it sends an ARP Request (broadcast) 
•	Destination replies with ARP Reply (unicast) 

 Switch MAC Address Learning
A switch works at the Data Link Layer and uses MAC addresses to forward frames.
•	When a frame arrives, the switch: 
o	Learns the source MAC address 
o	Stores it in the MAC address table 
•	If destination MAC is unknown: 
o	Switch sends data to all ports (broadcast) 
•	If known: 
o	Switch sends data only to the correct port 

 Simulation Mode
Simulation Mode in Packet Tracer allows:
•	Step-by-step visualization of packet movement 
•	Observation of protocols like ARP and ICMP 
•	Viewing packet details in the event list 
•	Understanding how devices process and forward packets 

 First Ping vs Second Ping
•	First Ping: 
o	Includes ARP + ICMP 
o	Takes more time 
•	Second Ping: 
o	Uses cached MAC address 
o	Only ICMP packets 
o	Faster communication
Basic Setup 
Task 1: Build a Simple LAN
1.	Open Cisco Packet Tracer 
2.	Add devices: 
o	1 Switch (2960) 
o	3 PCs (PC0, PC1, PC2) 
3.	Connect using Copper Straight Through Cable: 
o	PC0 → Switch 
o	PC1 → Switch 
o	PC2 → Switch 
4.	Assign IP Addresses to PCs

 
Task 2: First Ping Observation
1.	Switch to Simulation Mode 
2.	Click Add Simple PDU 
3.	Click: 
Source: PC0 
Destination: PC1

 


Step-by-step flow:
1.	ARP Request (Broadcast) 
o	PC0 → "Who has 192.168.20.2?" 
o	Sent to all devices via switch 
2.	Switch Behavior 
o	Learns MAC of PC0 (source) 
o	Forwards broadcast to all ports 
3.	ARP Reply (Unicast) 
o	PC1 → "I am 192.168.20.2" 
o	Sent only to PC0 
4.	ICMP Echo Request 
o	PC0 sends ping 
5.	ICMP Echo Reply 
o	PC1 replies


Task 3: Second Ping Observation
Repeat ping (PC0 → PC1)

 


 What changes:
•	 No ARP request this time 
•	 Direct ICMP packets only 
Reason:
•	ARP entry is stored in cache (memory)


Task 4: MAC Table Check
1.	Click Switch 
2.	Go to CLI 
3.	Press Enter 
4.	Type: 
enable
show mac address-table

 
















