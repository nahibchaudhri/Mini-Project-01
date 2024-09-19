## Mini-Project-01

## 1. System Architecture Diagram
![Screenshot (3)](https://github.com/user-attachments/assets/b5aaf161-6da2-4c54-85de-cb59073391d5)

## 2. Step-by-step Configuration Guide
_The Network_
The diagram shows a network with two main subnets: 192.168.0.0/24 (the ISBA Lab
LAN) and 172.16.0.0/16 (the UHail Data Center LAN).
_Devices:_
The devices include:
_Server:_
Web Server, DNS Server, Server2
_Switches:_
One switch connecting Fa0/1, Fa0/2, Fa0/3, and Fa0/4
_Pc:_
PC1, PC2, PC3, PC4
_Others:_
Smartphone, Laptop, Tablet PC, Access Point
_Connections:_
- The network has two separate subnets, with a few devices connecting them.
- The ISBA Lab LAN has PCs connected to the switch through Fa0/1 and Fa0/2.
- The UHail Data Center LAN has a web server, DNS server, and Server2 connected
to the switch.
- The Smartphone, Laptop, and Tablet PC are connected to the Access Point, which
is on the ISBA Lab LAN.
- There is a connection between the two subnets using Fa0 and Fa0/4, connecting the
switch to the DNS Server.

_Diagram of the network_
![Screenshot (4)](https://github.com/user-attachments/assets/1cc2956b-2775-43d7-ae7c-dad37236d960) 


_Images of the Connection_ (ping command being used)
![Screenshot (5)](https://github.com/user-attachments/assets/6555062f-4a2d-4c39-bf8f-ec87f2eb251f) 

_Image of simulation_
![Screenshot (6)](https://github.com/user-attachments/assets/8bc28b82-597f-4061-8602-092479fae76d) 

- The switches are important for providing connectivity to devices within the same LAN
- The diagram shows that the switches do not provide connectivity between the two LANS.

- The diagram presents a basic network setup with two separate subnets and devices
connected through a switch. The layout highlights the importance of switches for
local connectivity and how connections between subnets are handled separately.

_HOW TO DO THIS MINI PROJECT_

1) SETTING UP THE NETWORK IN PACKET TRACER

   _Devices_
   Routers: Create a router for the "UHail Data Center LAN" (likely representing a larger network). It will have an interface connected to the internet (outside world) and a separate interface connected to the rest of your network.

  Switch: Use a switch for the "ISBA Lab LAN" (a LAN for internal network communication).

  Computers: Create PCs for each device labeled "PC" in the diagram (PC1, PC2, PC3, PC4).

  Servers: You'll need a server for the "Web Server" and another for the "DNS Server."

   _Interfaces:_
  Router: Connect your router's interface to your switch (e.g., GigabitEthernet0/0 on the router
might connect to FastEthernet0/0 on the switch).

  Switch: Connect your switch's ports (e.g., FastEthernet0/1, FastEthernet0/2, etc.) to your PCs and servers.
  Servers: Connect each server to a different port on the switch.

 _IP Addressing:_
- UHail Data Center LAN (Router): Choose an IP address from the "Usable IPs" range (172.16.0.1 - 172.31.255.255).
- Important: Use a subnet mask of 255.255.0.0 (subnet mask is not shown in your diagram).
- Example: 172.16.1.1/255.255.0.0
- ISBA Lab LAN (Switch): Choose an IP address from the "Usable IPs" range (192.168.0.1 - 192.168.0.254).
- Important: Use a subnet mask of 255.255.255.0.
- Example: 192.168.0.10/255.255.255.0
- PCs and Servers: Assign IP addresses from their respective subnets, ensuring no IP
addresses are duplicated.
  _Connectivity:_
- Router to Switch: Make sure the router and switch are connected and able to communicate.
- Switch to Devices: All PCs and servers should be able to communicate with each other
through the switch.

2) CONFIGURATION
- Router: Configure your router to be a gateway for the ISBA Lab LAN.
- Enable and configure NAT (Network Address Translation) on the router to allow devices on the ISBA Lab LAN to access the internet.
  _Switch:_
- VLANs: If you want to segment your network further, you could configure VLANs on your
  switch.

3) TESTING
  - Ping: Use the ping command to test connectivity between devices.
  - Telnet: Use telnet (if allowed by your network setup) to test connection to 
    servers and the internet.

KEY CONCEPTS 
- IP Addressing: Ensure all devices have unique IP addresses and use the correct subnet mask.
- Subnet Mask: Subnet masks are used to identify the network portion of an IP address,
helping devices route traffic within the same network.
- Gateway: The router acts as a gateway between the ISBA Lab LAN and the "UHail Data
Center LAN" or the external network.
- NAT: NAT is used to translate private IP addresses used on the ISBA Lab LAN to a public IP address used by the router for communication with the outside world.

## 3. FAQ

1. What type of connection is used between the PCs and the Switch?
Answer - The connection between the PCs and the Switch is an Ethernet connection, as indicated by the "Fa0" (Fast Ethernet) interface labels on the devices

2. What is the purpose of the Switch in this network?
Answer - The Switch acts as a central point for connecting all the devices on the network. It facilitates communication between them by learning the MAC addresses of each device and forwarding data packets to the correct destination.

3. What is the purpose of the Access Point? 
Answer - The Access Point provides a wireless connection to the network for the Laptop and the Smartphone. It acts as a bridge between the wired network and the wireless devices.

4. What is the difference between the ISBA Lab LAN and the UHail Data Center LAN? 
Answer - The two networks have different network addresses and different subnet masks. The ISBA Lab LAN is a Class C network with a subnet mask of /24, while the UHail Data Center  LAN is a Class B network with a subnet mask of /16. This means that the UHail Data Center  LAN has a larger number of usable IP addresses than the ISBA Lab LAN. 

5. Why is the Web Server connected to the Switch and not directly to a PC? 
Answer - The Web Server is connected to the Switch to provide access to all the devices on the network. Connecting it directly to a PC would limit access to only that specific PC,  making it difficult for other devices to access the Web Server.





## 4. Reflection 

One of the main challenges in setting up this network was ensuring that all devices  were properly connected and configured. This involved assigning the correct IP  addresses, subnet masks, and default gateways to each device. Additionally,  configuring the switches to forward traffic correctly was crucial. 
To overcome these challenges, I relied on my understanding of basic network  concepts, such as IP addressing, subnetting, and routing. I also utilized the Cisco 
Packet Tracer simulation to visualize and test the network setup, which helped  identify and resolve any configuration issues. 
Through this project, I gained a deeper understanding of network fundamentals,  including LANs, IP addressing, and connectivity. I also developed my skills in  configuring and troubleshooting network devices using the Cisco Packet Tracer  simulation. 
One idea possibly for the future is adding more complexity to the network setup, such as  incorporating routers, firewalls, or virtual private networks (VPNs). This would allow  for a more comprehensive understanding of network security and scalability. 
Additionally, exploring different network topologies, such as mesh or ring topologies,  could provide valuable insights into network design and optimization.


