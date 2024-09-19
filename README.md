## Mini-Project-01

## 1. System Architecture Diagram
https://github.com/nahibchaudhri/Mini-Project-01/issues/1#issue-2536726668 
## 2. Step-by-step Configuration Guide

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


