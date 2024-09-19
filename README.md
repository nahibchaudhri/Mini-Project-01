## Mini-Project-01

## 1. System Architecture Diagram
![Screenshot (3)](https://github.com/user-attachments/assets/b5aaf161-6da2-4c54-85de-cb59073391d5)

## 2. Step-by-step Configuration Guide
_The Network__
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


