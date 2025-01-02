


## Project Overview
This project is part of the Communications & Network Fundamentals course at Imam Abdulrahman Bin Faisal University. 
The objective is to design, configure, and test a network topology using Cisco Packet Tracer. 
The network consists of multiple routers, switches, and end devices connected across different LAN segments. 
The focus is on implementing basic IP addressing, configuring routing between networks, and ensuring smooth communication between devices.

## Topology Demonstration
The following topology was designed and configured as part of the project:

![image](https://github.com/user-attachments/assets/c6aa947d-7ec5-4b5c-83a5-5f26d103075b)


## Addressing Table
The addressing table below outlines the IP addresses, subnet masks, and gateway configurations for all devices in the network.

| Device        | Interface | IP Address  | Subnet Mask   | Default Gateway |
|--------------|-----------|-------------|---------------|-----------------|
| Router0      | F0/0      | 192.168.0.1 | 255.0.0.0     | N/A             |
| Router0      | Se1/0     | 10.1.1.1    | 255.0.0.0     | N/A             |
| Router0      | Se3/0     | 11.1.1.1    | 255.0.0.0     | N/A             |
| Router1      | F0/0      | 192.168.1.1 | 255.0.0.0     | N/A             |
| Router1      | Se1/0     | 10.1.1.2    | 255.0.0.0     | N/A             |
| Router1      | Se2/0     | 12.1.1.1    | 255.0.0.0     | N/A             |
| Router2      | F0/0      | 192.168.2.1 | 255.0.0.0     | N/A             |
| Router2      | Se0/3/0   | 11.1.1.2    | 255.0.0.0     | N/A             |
| Router2      | Se0/3/1   | 12.1.1.2    | 255.0.0.0     | N/A             |
| Server0      | F0/0      | 192.168.0.4 | 255.255.255.0 | 192.168.0.1     |
| PC0          | F0/0      | 192.168.0.2 | 255.255.255.0 | 192.168.0.1     |
| PC1          | F0/0      | 192.168.1.2 | 255.255.255.0 | 192.168.1.1     |
| PC2          | F0/0      | 192.168.1.3 | 255.255.255.0 | 192.168.2.1     |
| PC3          | F0/0      | 192.168.2.3 | 255.255.255.0 | 192.168.2.1     |
| Laptop0      | Wireless  | 192.168.0.5 | 255.255.255.0 | 192.168.0.1     |
| Laptop1      | Wireless  | 192.168.1.5 | 255.255.255.0 | 192.168.1.1     |
| Laptop2      | F0/0      | 192.168.2.2 | 255.255.255.0 | 192.168.2.1     |
| Laptop3      | F0/0      | 192.168.2.4 | 255.255.255.0 | 192.168.2.1     |

## Configuration Steps

### 1. Equipment Setup
- Place routers, switches, and end devices in Cisco Packet Tracer according to the topology diagram.
- Use appropriate cabling to connect the routers via serial interfaces and connect end devices to switches using copper straight-through cables.
- Ensure that wireless laptops are connected to the corresponding access points.

### 2. IP Addressing
- Configure static IP addresses and subnet masks on all end devices.
- Assign IP addresses to router interfaces to facilitate communication between networks.
- Verify that each PC, laptop, and server is configured with the correct default gateway (IP address of the router interface for that subnet).

### 3. Router Configuration
- Access each router using the console connection.
- Enter global configuration mode and configure each interface with the appropriate IP address and subnet mask.
- Enable the interfaces to bring them up and ensure they can communicate.
- Configure static or dynamic routing protocols to ensure inter-network connectivity.

### 4. Wireless Setup
- Configure wireless access points with SSIDs and enable AES encryption to secure wireless communication.
- Ensure laptops connect to the appropriate wireless network by providing the correct SSID and security key.

### 5. VoIP Configuration
- Assign IP addresses to IP phones using DHCP or static configuration.
- Connect IP phones to switches and verify their connectivity.
- Ensure that voice VLANs are configured if necessary, and phones are assigned to the correct VLAN.

### 6. Connectivity Testing
- Use the ping command from PCs and laptops to test connectivity to devices in different LANs.
- Ensure that devices from the blue network can reach devices in the orange and yellow networks.
- Troubleshoot connectivity issues by verifying cabling, IP addressing, and routing configurations.

## Verification
- Verify successful communication between networks by performing extended ping tests.
- Use traceroute commands to analyze the path of packets and ensure routers forward data correctly.
- Address any detected IP conflicts or misconfigurations to ensure seamless connectivity.

---

