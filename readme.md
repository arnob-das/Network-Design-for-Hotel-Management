# Network-Design-for-Hotel-Management

## Description
This project shows how to design and set up a network for Modern Hotel using Cisco Packet Tracer. The network connects three floors and eight departments. Each department uses its own VLAN to keep network traffic separate, secure, and easy to manage. Routers use OSPF to communicate between floors, and DHCP automatically assigns IP addresses to devices.

## Network Overview
* Floors: 3
* Departments: 8 (Reception, Store, Logistics, Finance, HR, Sales, Admin, IT)
* Devices: 3 Routers, 3 Switches, Access Points, Printers, PCs, and a Test PC
* Routing Protocol: OSPF
* Network Services: DHCP, SSH, Port Security, and WLAN

## VLAN and IP Addressing Table

| Floor | Department | VLAN ID | Network Address |
| --- | --- | --- | --- |
| 1st | Reception | 80 | 192.168.8.0/24 |
| 1st | Store | 70 | 192.168.7.0/24 |
| 1st | Logistics | 60 | 192.168.6.0/24 |
| 2nd | Finance | 50 | 192.168.5.0/24 |
| 2nd | HR | 40 | 192.168.4.0/24 |
| 2nd | Sales | 30 | 192.168.3.0/24 |
| 3rd | Admin | 20 | 192.168.2.0/24 |
| 3rd | IT | 10 | 192.168.1.0/24 |

## Features and Technologies
* Network Segmentation: Separate VLANs for each department.
* Inter-VLAN Routing: Uses Router-on-a-Stick for communication across VLANs.
* Dynamic Routing: OSPF connects the routers across all three floors.
* Automatic IP Assignment: Routers act as DHCP servers for connected devices.
* Secure Remote Access: SSH enabled for administrative access.
* Switch Security: Port Security enabled on the IT switch (port FastEthernet0/1 restricted to the Test PC).
* Wireless Access: WLAN setup for laptops and mobile devices.

## Testing and Results
* All devices receive dynamic IP addresses from the DHCP server.
* Ping tests confirmed successful communication between different VLANs.
* OSPF successfully routes traffic across all routers.
* Remote access via SSH was verified from the Test PC.
* Port Security was tested using sticky MAC addresses.
* Wireless devices connect properly to the Access Points.

## Project Files
* `Network Design for Hotel Management.pkt.pkt` - Cisco Packet Tracer network file located in the main folder.
* `screenshots/` - Contains the screenshot image of the project network layout.

## License
This project is released under the MIT License.
