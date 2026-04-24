Experiment 9: Transport Layer Simulation (TCP vs UDP)
1. Objective
Simulate process-to-process communication
Demonstrate working of:
TCP
UDP
Compare protocols based on:
Connection establishment
Data transmission
Congestion control
2. Network Topology
Components Required
PC
Switch
Server
Topology
PC ---- Switch ---- Server
3. IP Address Configuration

Assign IPv4 addresses:

PC
IP: 192.168.1.10
Subnet Mask: 255.255.255.0
Server
IP: 192.168.1.20
Subnet Mask: 255.255.255.0
4. TCP Simulation (HTTP Service)
Concept

TCP ensures reliable communication using a connection setup.

Steps
Open Server → Services → HTTP → ON
On PC:
Go to Desktop → Web Browser
Enter: http://192.168.1.20
Switch to Simulation Mode
Filter:
TCP
HTTP
What Happens (3-Way Handshake)
SYN → PC sends request
SYN-ACK → Server responds
ACK → Connection established
Observation
Reliable delivery
Ordered packets
Retransmission if failure
5. UDP Simulation (DNS Service)
Concept

UDP provides fast but unreliable communication.

Steps
On Server:
Go to Services → DNS
Turn ON DNS

Add:

Name: www.test.com
Address: 192.168.1.20
On PC:
Go to Desktop → IP Configuration
Add DNS Server: 192.168.1.20
Open Web Browser
Enter: www.test.com
Switch to Simulation Mode
Filter UDP + DNS
Observation
No connection setup
Direct request-response
Faster communication
6. Key Concepts Demonstrated
Transport Layer (Layer 4)

OSI model Layer 4 handles:

Port numbers (process identification)
Segmentation
Reliability
7. TCP vs UDP Comparison
Feature	TCP	UDP
Connection	Connection-oriented	Connectionless
Reliability	High	Low
Speed	Slower	Faster
Ordering	Maintained	Not guaranteed
Error Control	Yes	No
Congestion Control	Yes	No
8. Congestion Control
TCP
Uses algorithms like Slow Start
Adjusts transmission rate dynamically
Prevents network overload
UDP
No congestion control
Sends packets continuously
May cause packet loss
9. Simulation Mode Analysis

In Packet Tracer:

Observe packet flow:
TCP handshake packets
UDP direct transmission
Compare:
Number of packets
Delay
Reliability
10. Expected Results
TCP establishes connection before sending data
UDP sends data instantly without setup
TCP is slower but reliable
UDP is faster but may lose packets
