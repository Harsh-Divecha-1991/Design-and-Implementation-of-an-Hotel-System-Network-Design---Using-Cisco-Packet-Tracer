# Design-and-Implementation-of-an-Hotel-System-Network-Design---Using-Cisco-Packet-Tracer

## 📋 Overview

This project aims to design and implement a secure and efficient network infrastructure for a hotel management company using Cisco Packet Tracer. The network is designed to adhere to the principles of **Confidentiality, Integrity, and Availability (CIA)**, ensuring that the network is secure, reliable, and efficient.

Key components of the network include:

- **Local Area Network (LAN)**
- **Wide Area Network (WAN)**
- **Server Site**: Hosting DHCP, DNS, Web, and Email Servers

The network follows a hierarchical model with multiple security and performance features.

## ✨ Project Highlights

- **Hierarchical Network Design**: Implemented to provide redundancy and improve network efficiency.
- **Segregated Network Segments**: All departments are on separate network segments within the LAN.
- **Dual ISP Connections**: Core routers at HQ and Branch connect to two subscribed ISPs.
- **Secure Communication**: Utilizes Access Control Lists (ACLs) and Virtual Private Networks (VPNs).
- **Dynamic and Static IP Addressing**: DHCP servers dynamically allocate IP addresses, while server devices have static IPs.
- **Inter-VLAN Routing**: Configured on multilayer switches to enable communication across different VLANs.
- **Routing Protocol**: Open Shortest Path First (OSPF) used for advertising routes.

## 🌐 Network Topology

The network topology is designed as follows:

1. **Core Routers**: Each site (HQ and Branch) has one core router.
2. **Multilayer Switches**: Two at each site, configured for routing and switching.
3. **Access Switches**: Connect to each department, each with an estimated 60 users at HQ and 30 users at the Branch.
4. **Wireless Network**: Each department has its own wireless network.

![Hotel Management System](https://github.com/user-attachments/assets/dac49d3b-09e7-4ac6-a5fc-7f5501e1b834)

## 🧮 IP Addressing and Subnetting

- **Base Network**: 192.168.100.0
- Subnetting is carried out to allocate the correct number of IP addresses to each department.
- Public IP addresses are used for internet connectivity, with the following ranges allocated to ISPs:
  - 195.136.17.0/30
  - 195.136.17.4/30
  - 195.136.17.8/30
  - 195.136.17.12/30

## 🔒 Security Features

- **Access Control Lists (ACLs)**: Configured to control user access and secure communication.
- **Port Security**: Implemented on server site department switches to allow only one device per port.
- **SSH Configuration**: Secure remote login configured on all routers and multilayer switches.
- **Site-to-Site VPN**: Configured using IPSec to encrypt communication between HQ and Branch.
- **Port Address Translation (PAT)**: Configured to handle outbound traffic using ACL rules.

## ⚙️ Network Configuration

### Device Settings

- Hostnames, console passwords, enable passwords, and banner messages are configured.
- IP domain lookup is disabled for security.

### DHCP and DNS Configuration

- Dedicated DHCP servers provide dynamic IP addresses to network devices.
- DNS servers are configured to resolve domain names within the network.

### Inter-VLAN Routing

- Multilayer switches are configured to handle routing between different VLANs.

### Routing Protocols

- OSPF is configured as the routing protocol for route advertisement.
- Default static routing is used to forward traffic that does not match routing table entries.

## 🛠️ Technologies Implemented

- **Hierarchical Network Design**
- **Correct Cabling and Device Connectivity**
- **Basic Device Settings Configuration**
- **VLAN Creation and Port Assignment**
- **Subnetting and IP Address Allocation**
- **Inter-VLAN Routing (Switch Virtual Interface)**
- **Dedicated DHCP Server for Dynamic IP Allocation**
- **Secure Remote Access via SSH**
- **OSPF Routing Protocol Configuration**
- **NAT Overload (Port Address Translation PAT)**
- **Site-to-Site IPSec VPN**
- **Standard and Extended Access Control Lists**
- **Switch Port Security Configuration**
- **Wireless Network (Cisco Access Point) Setup**
- **Host Device Configuration**
- **ISP Router Configuration**

## 📖 How to Use

1. Clone the repository to your local machine.
2. Open the project file in Cisco Packet Tracer.
3. Review the network topology and configurations.
4. Modify and customize the network settings as needed for your environment.

## 📚 Additional Resources

- [Cisco Packet Tracer Documentation](https://www.netacad.com/courses/packet-tracer)
- [Networking Basics Guide](https://www.cisco.com/c/en/us/solutions/small-business/resource-center/networking/networking-basics.html)
