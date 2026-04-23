Experiment 4 :

Objective : Implement error detection and correction mechanisms using block coding and Cyclic Redundancy Check (CRC). Simulate a communication system in Cisco Packet Tracer to demonstrate how errors are detected and corrected during data transmission.

Components required : 
Hardware Components (in Cisco Packet Tracer):
•	1 Switch
•	2 PCs 
•	Cables (Copper Straight Through) 

Block Coding
•	Data is divided into blocks 
•	Extra bits (parity bits) are added 
•	Helps in: 
o	Error detection 
o	Single-bit error correction 
 Example:
Data: 1011 → Sent as 1011 + parity bit

 CRC (Cyclic Redundancy Check)
•	Uses a generator polynomial 
•	Sender adds CRC bits 
•	Receiver recalculates and compares 
 If mismatch → Error detected

Basic Setup
Steps:
1.	Build topology with: 
o	1 switch + 2 PCs 
2.	Assign IPs (same network) 
3.	Use Simulation Mode 
4.	Start  pings: 
o	PC0 → PC1 
5.	Introduce error
6.	Correct error
7.	Observe

 
 

 

 


 
