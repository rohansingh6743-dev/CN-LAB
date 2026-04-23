Experiment 5 :

Objective : Design and simulate flow control and error control protocols such as Stop and Wait, Go-Back-N ARQ, and Selective Repeat ARQ. Compare their performance in terms of throughput and efficiency under varying network conditions.
Components required : 
Hardware Components (in Cisco Packet Tracer):
•	1 Switch
•	2 PCs 
•	Cables (Copper Straight Through) 
In data communication, reliable transmission of data is very important. Two key mechanisms used to ensure reliability are flow control and error control.

Flow Control
Flow control ensures that the sender does not send data faster than the receiver can handle.
 If data is sent too fast:
•	Receiver buffer may overflow 
•	Packets may be lost 
 Therefore, flow control maintains a balanced data transmission rate.
 Error Control
Error control ensures that data is transmitted correctly without errors.
Errors may occur due to:
•	Noise in the communication channel 
•	Signal interference 
•	Network congestion 
Error control techniques:
•	Detect errors 
•	Retransmit lost or corrupted data 

ARQ Protocols (Automatic Repeat reQuest)
ARQ protocols are used for error detection and retransmission of lost or damaged frames.

 1. Stop and Wait ARQ
•	Sender sends one frame at a time 
•	Waits for acknowledgment (ACK) 
•	If ACK not received → retransmit 
Advantages:
•	Simple and reliable 
 Disadvantages:
•	Slow (low throughput) 

2. Go-Back-N ARQ
•	Sender can send multiple frames continuously 
•	Uses a window size 
•	If one frame is lost: 
•	All frames after it are retransmitted 
 Advantages:
•	Faster than Stop and Wait 
Disadvantages:
•	Wastes bandwidth (retransmits many frames) 

 3. Selective Repeat ARQ
•	Sender sends multiple frames 
•	Only incorrect or lost frames are retransmitted 
 Advantages:
•	High efficiency 
•	Better throughput 
 Disadvantages:
•	More complex

<img width="940" height="501" alt="image" src="https://github.com/user-attachments/assets/75d7b105-5249-4f52-83bc-c6bab240be5f" />

Basic Setup
Steps:
1.	Build topology with: 
o	1 switch + 2 PCs 
2.	Assign IPs (same network) 
3.	Use Simulation Mode 
4.	Start  pings: 
o	PC0 → PC1 

 

<img width="940" height="497" alt="image" src="https://github.com/user-attachments/assets/3d4e2166-19b0-47dc-a7cb-1963e09d2b8f" />

 


Stop and Wait:
- Slow transmission
- High delay
- Reliable but inefficient

Go-Back-N:
- Faster than Stop & Wait
- Retransmits multiple packets
- Moderate efficiency

Selective Repeat:
- Highest efficiency
- Only failed packets retransmitted
- Better throughput

Conclusion:
Selective Repeat ARQ provides best performance under error conditions.
