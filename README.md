# Smart Office Network Project

## Overview
This project designs and implements a **smart office network** that integrates IoT devices, advanced networking, and centralized server systems to enhance efficiency, security, and connectivity. The network supports two office environments, two home networks, and a VoIP system, all connected through a central router (Router4). The system ensures secure communication, dynamic IP allocation, and IoT automation for a modern, flexible work environment.

---

## Key Features
- **Centralized Server System**: Hosts DHCP, DNS, HTTP, FTP, and SMTP servers for seamless resource management.
- **Dynamic Routing**: Uses **RIP Version 2** for efficient routing between subnets.
- **IoT Integration**: Includes motion sensors, RFID doors, smart coffee machines, and AC systems for automation.
- **Access Control**: **ACLs** restrict direct communication between devices, ensuring all traffic passes through the server network for enhanced security.
- **Remote Work Support**: Home networks enable secure remote access and IoT device control.

---

## Network Design
### Components
1. **Office Networks**:
   - Two offices with PCs, printers, and switches connected to Router4.
   - IP ranges: `192.168.1.0/24` (Office 1) and `192.168.3.0/24` (Office 2).

2. **Home Networks**:
   - Two home networks with wireless routers and IoT devices.
   - IP ranges: `192.168.0.0/24` (Home 1) and `192.168.5.0/24` (Home 2).

3. **VoIP Network**:
   - IP phones connected via a switch and router.
   - IP range: `192.168.10.0/24`.

4. **Server Network**:
   - Centralized server room with DHCP, DNS, HTTP, FTP, and SMTP servers.
   - IP range: `192.168.2.0/24`.

5. **Central Router (Router4)**:
   - Connects all networks and enforces routing and security policies.

---

## Technologies Used
- **Cisco Packet Tracer**: For network simulation and configuration.
- **RIP Version 2**: For dynamic routing between subnets.
- **IoT Devices**: Motion sensors, RFID doors, smart coffee machines, and AC systems.
- **Server Software**: DHCP, DNS, HTTP, FTP, and SMTP servers for centralized management.
- **Access Control Lists (ACLs)**: To restrict direct communication between devices.

---

## Server Configuration
- **DHCP Server**: Dynamically assigns IP addresses to devices in all networks.
- **DNS Server**: Resolves hostnames (e.g., `web.smartoffice.local` → `192.168.2.10`).
- **Web Server**: Hosts a test page for internal web services.
- **FTP Server**: Enables secure file transfers across the network.
- **Email Server**: Handles internal email communication via SMTP.

---

## IoT Integration
- **Devices**: Motion sensors, RFID doors, smart coffee machines, and AC systems.
- **LAN Setup**: IoT devices operate on a dedicated LAN (`192.168.25.1`) with wireless connectivity.
- **Control**: All devices can be monitored and controlled via a smartphone IoT monitor.

---

## Security Features
- **Access Control Lists (ACLs)**: Block direct communication between devices, ensuring all traffic passes through the server network.
- **Centralized Routing**: All traffic flows through Router4, enhancing control and security.
- **IoT Security**: Devices operate on a dedicated LAN with restricted access.

---

## Future Improvements
1. **Scalability**: Replace RIP with OSPF or EIGRP for better performance in larger networks.
2. **Redundancy**: Implement HSRP to eliminate single points of failure.
3. **Enhanced Security**: Add firewalls and IPsec encryption for advanced protection.
4. **Network Monitoring**: Deploy tools like SNMP for real-time network management.

---

## Conclusion
This smart office network project successfully demonstrates centralized control, dynamic routing, and IoT integration for a modern, secure, and efficient work environment. By addressing scalability and security limitations, the network can be further improved for long-term performance.

---

## References
- **Cisco Packet Tracer**: Used for network simulation.
- **RIP Version 2**: For dynamic routing.
- **IoT Devices**: For automation and control.
- **Server Software**: For centralized resource management.
