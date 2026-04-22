Assignment 4: Transmission Failure Demonstration (Link Errors & Retransmission Idea)

Experiment Objectives
This experiment demonstrates practical “errors” in communication by forcing link failures during transmission and observing which packets fail and how communication resumes after recovery.

Components required : 
Hardware Components (in Cisco Packet Tracer):
•	1 Switch (2960) 
•	2 PC
•	Copper Straight Through cables 

In a computer network, communication depends on physical links (cables) and network devices. If a link fails (e.g., cable unplugged), data transmission is interrupted.
This leads to:
•	Packet loss (data not delivered) 
•	Timeouts (no response received) 
•	Communication failure 
•	When the link is restored, communication resumes, showing how networks recover after failure.

 ICMP Behavior During Failure
•	ICMP (ping) is used to test connectivity 
•	During normal conditions → Reply received 
•	During failure → Request timed out 

 Simulation Mode Role
Simulation Mode helps to:
•	Visualize packet drops 
•	Observe failed transmissions 
•	Understand recovery 


Basic Setup 
Task 1: Setup
1.	Open Cisco Packet Tracer 
2.	Add devices: 
o	1 Switch (2960) 
o	2 PCs (PC0, PC1) 
3.	Connect using Copper Straight Through Cable: 
o	PC → Switch 
4.	Assign IP Addresses to both PCs
 
<img width="788" height="417" alt="image" src="https://github.com/user-attachments/assets/7770f21f-b0b6-4c37-98bc-320736b519e8" />




Task 2: Normal Communication
Ping PC0-PC1
 <img width="929" height="493" alt="image" src="https://github.com/user-attachments/assets/7a478579-ed2d-4dae-8b75-548d38b993a4" />


Observe in Simulation:
•	Replies received 
•	Communication successful
 

Task 3: Force Error
1.	Start continuous ping:  PC0-PC1
2.	While ping is running: 
o	Disconnect cable between PC1 and Switch
<img width="914" height="486" alt="image" src="https://github.com/user-attachments/assets/813bae17-b6fa-4f99-aea7-e3608b040626" />

 

Observation:
•	“Request timed out” 
•	Packets fail in Simulation Mode 
•	Red indicators (packet drops)


Task 4: Recovery
•	Reconnect the cable 
•	Observe ping output
<img width="776" height="411" alt="image" src="https://github.com/user-attachments/assets/1a1622c8-3d04-4c03-a53d-4b3476f86483" />


 

Observation:
•	Replies start coming again 
•	Communication restored








