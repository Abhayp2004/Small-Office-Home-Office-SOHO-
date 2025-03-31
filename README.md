Simple Office Home Office (SOHO) Network Setup
Overview
This project focuses on designing and setting up a Simple Office Home Office (SOHO) network using Cisco Packet Tracer. The goal is to create a network that connects devices within a small-scale office or home environment, allowing them to communicate, share resources, and access the internet.

The network design includes multiple departments like the Chairman’s Office, IT Department, Computer Department, and Server Room, all connected via a central router. Each department is assigned a unique subnet, and various devices such as computers, printers, and switches are structured for optimal communication and resource sharing.

Network Topology Overview
The network uses a star topology, with a central router acting as the hub connecting the various departments via dedicated switches. Below is the breakdown of each department:

Departments and Devices:
Chairman Department

Devices: Chairman’s computer, VC computer

Subnet: 192.168.1.0/24

Switch: Chairman Switch

IT Department

Devices: Employee Computers (4, 5), IT Department Printer, Manager Computer 2

Subnet: 192.168.2.0/24

Switch: IT Department Switch

Computer Department

Devices: Employee Computers (1, 2, 3), Manager Computer 1, Computer Department Printer

Subnet: 192.168.3.0/24

Switch: Computer Department Switch

Server Room

Devices: Server 0, Laptop 0

Subnet: 1.0.0.0/24

Switch: Server Room Switch

Each department is connected to the central router, which has multiple network interfaces to manage inter-department routing and external connections.

Network Setup
Step 1: Subnet Design
Each department is assigned a unique subnet to facilitate network management:

Chairman Department: 192.168.1.0/24

IT Department: 192.168.2.0/24

Computer Department: 192.168.3.0/24

Server Room: 1.0.0.0/24

Router interfaces are configured as:

192.168.1.1 (Chairman Department)

192.168.2.1 (IT Department)

192.168.3.1 (Computer Department)

1.0.0.1 (Server Room)

Step 2: Device Configuration
Assign static IP addresses to all devices in their respective subnets.

Example: Chairman's computer: 192.168.1.2, VC computer: 192.168.1.3.

Step 3: Switch Setup
Each department has a dedicated switch.

The switches connect devices within the department and route traffic to the central router for inter-department communication.

Step 4: Router Configuration
Configure static routes on the router to enable communication between departments:

Routing between 192.168.1.0/24 (Chairman Department), 192.168.2.0/24 (IT Department), 192.168.3.0/24 (Computer Department), and 1.0.0.0/24 (Server Room).

Step 5: DNS Configuration
Set up DNS server services to enable easy access to network resources via domain names.

Step 6: Testing the Network
Test connectivity by pinging between devices in different departments to ensure routing is correctly configured.

Step 7: Testing the Server Web Access
Open a browser from any department PC and enter the URL configured in the DNS server to verify web server access.

Conclusion
This SOHO network design provides a simple, efficient, and scalable solution for small offices or home office environments. The network topology ensures that communication between departments is smooth and isolated to optimize performance and security.

Key highlights include:

Segmentation: Different subnets for each department to enhance security and traffic management.

Centralized Services: DHCP and DNS for simplified management.

Expandable: Future devices and departments can be added with minimal reconfiguration.

The design is easy to implement, and the network offers room for future expansion as the office grows.

Technologies Used
Cisco Packet Tracer: For designing and simulating the network.

Cisco Routers and Switches: Used to build the network and route traffic between departments.

DNS Services: For managing domain name resolution within the network.
