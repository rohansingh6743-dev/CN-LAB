Experiment 10: DNS and DDNS Simulation
1. Objective
Demonstrate domain name resolution
Simulate:
DNS
DDNS
Create a client-server setup for querying and updating DNS records
2. Components Required
1 Switch (2960)
2 Servers:
DNS Server
Web Server
1 PC
Copper Straight-through cables
3. Network Topology
PC ---- Switch ---- DNS Server
              |
              ---- Web Server
4. IP Address Configuration

Assign IPv4 addresses:

PC
IP: 192.168.1.10
Subnet Mask: 255.255.255.0
DNS: 192.168.1.20
DNS Server
IP: 192.168.1.20
Web Server
IP: 192.168.1.30
5. DNS Server Configuration
Click DNS Server
Go to Services → DNS
Turn DNS → ON
Add record:
Name: www.payal.com
Address: 192.168.1.30
Concept

DNS maps:

www.payal.com → 192.168.1.30
6. Web Server Configuration
Click Web Server
Go to Services → HTTP
Turn HTTP → ON
Edit HTML page:
Welcome to Payal Website
DNS Simulation Successful!
7. Client (PC) Configuration
Go to Desktop → IP Configuration
Set:
DNS Server: 192.168.1.20
Open Web Browser
Type:
www.payal.com
8. Testing DNS Resolution
Expected Result
DNS resolves domain name to IP
Web page loads successfully
Simulation Mode

Switch to Simulation Mode and filter:

DNS
HTTP
Observe
DNS Query (PC → DNS Server)
DNS Response (IP returned)
HTTP Request to Web Server
9. DDNS Simulation (Dynamic Update)
Concept

DDNS updates DNS records when IP changes.

Steps to Simulate DDNS
Change Web Server IP:
From: 192.168.1.30
To: 192.168.1.40
Update DNS Record:
Go to DNS Server → Services → DNS

Modify:

www.payal.com → 192.168.1.40
Test again from PC:
Open browser → www.payal.com
Observation
Without update → website fails
After update → works again
10. DNS vs DDNS
Feature	DNS	DDNS
Update Type	Manual	Automatic
IP Change Handling	Needs manual update	Auto updates
Use Case	Static servers	Dynamic IP systems
11. Key Learning
DNS converts domain names into IP addresses
DDNS ensures updated mappings when IP changes
Client-server model enables name resolution
Real-world internet depends heavily on DNS
12. Expected Result
Successful DNS resolution
Website accessible via domain name
DDNS simulation shows dynamic update behavior
