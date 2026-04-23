Experiment 3 :

Objective : Develop a network simulator to analyze packet delay, loss, and end-to-end throughput. Implement various routing algorithms and measure their impact on network performance under different traffic conditions.
Components required : 
Hardware Components (in Cisco Packet Tracer):
•	2 Switches 
•	2 Router 
•	4 PCs 
•	Cables (Copper Straight Through) 

A network simulator helps analyze how data travels across a network and measures key performance metrics:
 Packet Delay
Time taken by a packet to travel from source to destination.
 Packet Loss
Occurs when packets fail to reach the destination due to:
•	Congestion 
•	Link failure 
•	Buffer overflow 
Throughput
Amount of data successfully delivered over time.
 Higher throughput = better performance
Basic Setup
Packet Switching Simulation
Steps:
1.	Build topology with: 
o	2 switches + 4 PCs 
2.	Assign IPs (same network) 
3.	Use Simulation Mode 
4.	Start multiple pings: 
o	PC0 → PC3 
o	PC1 → PC2 




 



Observation:
•	Packets move simultaneously 
•	Share same links 
•	Possible delay under load


Circuit Switching Simulation

Steps:
1.	Allow only one ping at a time 
2.	Stop other traffic 
3.	Send: 




 Observation:
•	No interference 
•	Smooth communication 
•	No packet collision

