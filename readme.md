# Banking Networking Project

## Overview
This project is designed to create a professional and secure network for a banking environment using **Cisco Packet Tracer**. The network demonstrates advanced networking concepts and configurations that can be used in any enterprise setting. It is a practical representation of how a bank's multiple departments and devices can interconnect, communicate, and function efficiently while maintaining high levels of security and redundancy.

---

## Purpose of the Project
1. **Efficient Communication:**  
   Ensure seamless communication between departments across four floors of the bank.

2. **Redundancy:**  
   Maintain network availability even if some devices or links fail.

3. **Security:**  
   Protect sensitive banking data and control access to the network using VLANs, port security, and SSH.

4. **Automation:**  
   Simplify network management by automating IP address allocation using a dedicated DHCP server.

5. **Scalability:**  
   Design a network that can grow with the bank’s future needs.

---

## Project Working

### 1. Network Design and Topology
- **Four Floors of the Bank:**  
  Each floor is equipped with a **router** and a **Layer 3 switch** to manage devices and network traffic efficiently.

- **Departments:**  
  The bank has **12 departments**, including Administration, IT, Marketing, Finance, etc., spread across the floors. Each department has both wired and wireless devices.

- **Guest Area:**  
  The 3rd floor includes a guest area with 40 devices and 2 printers.

- **Server Room:**  
  Located on the 4th floor, the server room hosts critical servers:
  - **DHCP Server:** Automatically assigns IP addresses.
  - **HTTP Server:** Provides web services.
  - **Email Server:** Manages communication within the bank.

---

### 2. VLAN Configuration
- **Purpose:**  
  VLANs (Virtual Local Area Networks) segment the network into isolated groups to improve performance and security. Each department is assigned a VLAN (e.g., VLAN 10 for Finance, VLAN 20 for HR).

- **Subnets:**  
  Each VLAN is allocated a unique IP subnet based on the number of devices in the department. This ensures efficient IP address management.

- **Routing Between VLANs:**  
  **Inter-VLAN Routing** is implemented using Layer 3 switches or routers to enable communication between VLANs.

---

### 3. IP Addressing
- **Automatic Allocation:**  
  All devices receive IPv4 addresses from the dedicated **DHCP server** in the server room. Static IPs are reserved for critical devices like servers and routers.

- **Subnet Mask:**  
  Each VLAN has a specific subnet mask and a reusable IP address range to optimize address allocation.

---

### 4. Security Implementation
- **Port Security:**  
  - Configured on switches to allow only specific devices to connect to each port using **sticky MAC addresses**.  
  - If an unauthorized device connects, the port goes into **shutdown mode** to prevent security breaches.

- **SSH (Secure Shell):**  
  - Enables secure remote management of routers.
  - Replaces insecure methods like Telnet.

- **Banner Messages:**  
  Display security warnings on all devices to deter unauthorized users.

- **Disabled Domain Lookup:**  
  Prevents delays caused by incorrect domain name resolution.

---

### 5. Routing Protocol
- **OSPF (Open Shortest Path First):**  
  A dynamic routing protocol used to advertise and manage routes between routers. It ensures efficient data transfer across the network.

---

### 6. Wireless Network
- **Purpose:**  
  Supports laptops, mobile devices, and other wireless equipment.  
- **Configuration:**  
  Wireless access points are secured with passwords to prevent unauthorized access.

---

### 7. Redundancy
- **Goal:**  
  To ensure the network remains operational even during device or link failures.  
- **Implementation:**  
  Backup paths and redundant devices are configured to reroute data automatically in case of failure.

---

## Things Implemented in the Project

1. **VLANs:**  
   Separate departments for better security and performance.
   
2. **Inter-VLAN Routing:**  
   Allows communication between VLANs.

3. **Port Security:**  
   Protects switch ports from unauthorized access.

4. **SSH:**  
   Enables secure remote login.

5. **DHCP Server:**  
   Automates IP address assignment.

6. **Static and Dynamic IP Configuration:**  
   Critical devices use static IPs; others use dynamic IPs.

7. **OSPF Routing Protocol:**  
   Ensures efficient and scalable data routing.

8. **Wireless Configuration:**  
   Supports wireless devices with secure connectivity.

9. **Redundancy:**  
   Keeps the network operational during failures.

---

## Project Outcome
By implementing this network, the bank achieves:
- **Security:** Sensitive data is protected through VLANs, port security, and ACLs.
- **Reliability:** Redundant paths ensure uninterrupted operations.
- **Efficiency:** Proper IP management and routing protocols optimize performance.
- **Scalability:** The network can easily accommodate growth in the future.

This project demonstrates professional networking practices that are essential for a modern banking environment. It combines theoretical knowledge with practical skills, making it a complete and reliable solution for enterprise-level networking.

