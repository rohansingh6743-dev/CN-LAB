Experiment 8: Logical Addressing & Address Mapping (IPv4 & IPv6)
1. Objective
Demonstrate logical addressing using IPv4 and IPv6
Simulate ARP, RARP, BOOTP, and DHCP processes
Visualize address resolution using simulation mode
2. Topology Design

Create a simple network:

1 Router
1 Switch
3–4 PCs
1 Server (for DHCP/BOOTP)
PC1 ----|
PC2 ----|        |---- Router ---- (Optional Internet)
PC3 ----| Switch |
                |---- Server
3. IPv4 Addressing Setup
Step 1: Assign Static IP (Manual)

On PCs:

IP: 192.168.1.x
Subnet Mask: 255.255.255.0
Gateway: 192.168.1.1

On Router:

enable
configure terminal
interface fastEthernet0/0
ip address 192.168.1.1 255.255.255.0
no shutdown
4. Demonstrating ARP (Address Resolution Protocol)
Concept

ARP maps IP → MAC address

Steps
Go to Simulation Mode

From PC1, ping PC2:

ping 192.168.1.2
Observe:
ARP Request (broadcast)
ARP Reply (unicast)
What You’ll See
PC1 asks: “Who has 192.168.1.2?”
PC2 replies with MAC address
5. Demonstrating RARP
Concept

RARP maps MAC → IP

Note
Not directly supported in Packet Tracer (obsolete in real networks)
You can explain it theoretically:
Used by diskless workstations
Replaced by DHCP/BOOTP
6. BOOTP Configuration
Concept

BOOTP assigns IP using MAC mapping

Steps
Use Server → Services → BOOTP
Add entry:
MAC Address of PC
Assign fixed IP (e.g., 192.168.1.10)
Set PC to BOOTP mode
Observation
Device gets predefined IP based on MAC
7. DHCP Configuration
Concept

DHCP dynamically assigns IPs

Steps (Server-based DHCP)
Click Server → Services → DHCP
Configure:
Pool Name: LAN
Default Gateway: 192.168.1.1
DNS: 8.8.8.8
Start IP: 192.168.1.100
Subnet Mask: 255.255.255.0
On PCs:
Select DHCP
Simulation Observation
DHCP Discover
DHCP Offer
DHCP Request
DHCP Acknowledgment
8. IPv6 Addressing Setup
Router Configuration
enable
configure terminal
ipv6 unicast-routing
interface fastEthernet0/0
ipv6 address 2001:db8:1::1/64
no shutdown
PC Configuration
Set IPv6 to Auto Config
Concept Demonstrated

IPv6 supports:

SLAAC (Stateless Address Auto Configuration)
No ARP (uses Neighbor Discovery Protocol instead)
9. Simulation Mode Analysis

Switch to Simulation Mode and filter:

ARP
DHCP
ICMP
Observe
Packet flow
Broadcast vs Unicast
Address resolution steps
10. Expected Results
Successful IPv4 communication using ARP
DHCP dynamically assigns IP addresses
BOOTP assigns fixed IP via MAC
IPv6 auto-configures addresses
Clear visualization of address resolution
