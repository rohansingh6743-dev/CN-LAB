Assignment 3: Effect of Network Load on Delay and Packet Drops

Experiment Objectives
Students will generate simultaneous traffic in a LAN to observe increased delays and packet drops under higher load. The focus is on interpreting simulation behavior rather than complex measurements.

Components required : 
Hardware Components (in Cisco Packet Tracer):
•	1 Switch (2960) 
•	6 PC
•	Copper Straight Through cables 

In a network, when multiple devices send data at the same time, the network experiences load (traffic). As the load increases, devices like switches must handle more packets, which can cause:
•	Delay (latency) → packets take longer to reach destination 
•	Queueing → packets wait in buffer 
•	Packet drops → packets are discarded when buffer is full 
This situation is called network congestion.

 ICMP Traffic
ICMP (used by ping) helps test connectivity and measure delay.
•	Low traffic → fast replies 
•	High traffic → delayed or lost replies 

Congestion in LAN
Even in a simple LAN:
•	Multiple simultaneous transmissions → shared bandwidth 
•	Switch queues get filled 
•	Results in delay or packet loss 

 Simulation Mode
Using simulation mode:
•	You can observe packet timing 
•	See how packets are delayed or dropped 
•	Analyze network behavior step-by-step 

Basic Setup 
Task 1: Baseline Test (Low Traffic)
1.	Open Cisco Packet Tracer 
2.	Add devices: 
o	1 Switch (2960) 
o	6 PCs (PC0, PC1, PC2, PC3,PC4,PC5) 
3.	Connect using Copper Straight Through Cable: 
o	PC → Switch 
4.	Assign IP Addresses to all PCs
5.	 Switch to Simulation Mode 
6.	  Ping from:PC0 → PC5
Observe: 
•	Smooth packet flow 
•	No delay 
•	No packet drops
 

 


Task 2: High Traffic Test
Start multiple pings at the same time:
•	PC0 → PC5 
•	PC1 → PC4 
•	PC2 → PC3 

Observe in Simulation:
•	Packets overlap 
•	Delay increases 
•	Some packets may be dropped 
•	Event list becomes crowded
  

 


Task 3: Observation Summary
Low Traffic:
•	Smooth communication 
•	No packet loss 
•	Fast response time 
 High Traffic:
•	Increased delay 
•	Packet queueing observed 
•	Some packet drops possible 
•	Slower response time
