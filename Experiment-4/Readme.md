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
<img width="580" height="308" alt="image" src="https://github.com/user-attachments/assets/b7500e6c-c007-4687-bf0e-e40ece44ea00" />

 <img width="851" height="452" alt="image" src="https://github.com/user-attachments/assets/e8dccb1c-211f-4471-82c3-7318520b0c94" />
<img width="863" height="458" alt="image" src="https://github.com/user-attachments/assets/373969c1-7ab7-4776-9f40-30253163127d" />
<img width="848" height="452" alt="image" src="https://github.com/user-attachments/assets/afc21f35-76d6-4fbc-b072-c724e0c2f88d" />
<img width="940" height="500" alt="image" src="https://github.com/user-attachments/assets/4deb3558-46e0-4bb3-982b-f9e0fd8d4b31" />

 

 

 


 
