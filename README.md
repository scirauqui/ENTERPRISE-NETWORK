# ENTERPRISE-NETWORK
This repository refers to an enterprise network simulation using Cisco Packet Tracer. 
The main objective of this project was to design a secure network by separating departments, providing automatic IP allocation, implementing dynamic routing and efficient addressing. It also offers controlled connectivity, default routes and access control lists, as well as network addresses translation.

Scalability was another key design objective. This network architecture allows the enterprise to add new departments and/or hosts if needed with minimal configuration changes. This can be done easily due to the segmentation of the company into different departments, reduced IP address waste and automatic IP allocation.

<img width="900" height="627" alt="image" src="https://github.com/user-attachments/assets/bea50eaf-b711-468f-944b-c69ceccaef7d" />


# TOPOLOGY
Regarding the network topology, it consists of:
  - 3 Cisco 2911 routers
  - 3 Cisco 2960 switches
  - 6 end devices
  - 3 VLANs
  - 2 WAN links

# NETWORK DESIGN
The design decisions taken regarding this specific network have been previously planned.

The VLANs were implemented so the departments are separated logically, thus reducing broadcast traffic and improving scalability and security.

APPLIED PROTOCOLS AND RULES:

VLSM and OSPF were applied to optimize IPv4 address allocations according to the number of hosts in each department, and to offer faster and better scalability, respectively.

DHCP automates the host configuration, which simplifies network administration.

The implementation of ACLs allows to enforce security policies. This way, guests are not able to access internal company resources.

Lastly, the PAT application allows multiple internal devices to use and share one single IP address to access Internet.

# FUTURE IMPROVEMENTS
Taking a look into the future, it would be interesting to implement HSRP to provide gateway redundancy and improve network availability and to introduce IPv6.

# TECHNOLOGIES
Cisco IOS, Cisco Packet Tracer, VLAN, Router-on-a-Stick, VLSM, RIP v2, OSPF, DHCP, ACL, NAT/PAT.





