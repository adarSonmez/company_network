# 🖧 Company Network Project in Cisco Packet Tracer

## Description

An enterprise company has hired you to set up a LAN for their new headquarters in Krakow. The following are the requirements and the solution implemented for the network in the new building:

1. **Cisco Packet Tracer Implementation:**  
   The entire network topology and configuration are created and simulated in Cisco Packet Tracer.

2. **IP Addressing:**  
   The company has allocated the network address `192.168.1.0/20` for the headquarters.

3. **Building Structure & VLANs:**  
   - The building consists of **4 floors**.
   - Each department operates on a separate floor and is assigned a unique VLAN and subnet.
   - VLANs are used to logically segment the network by department.

4. **Wireless Connectivity:**  
   - The third floor features a **wireless access point** supporting up to 1000 devices.
   - WPA2-PSK authentication is configured; only devices with the correct password can connect.

5. **Core Routing & Switching:**  
   - A **core router** connects the LAN to the ISP.
   - **Two multilayer switches** are connected to the core router.
   - **Inter-VLAN Routing** is configured on the multilayer switches to allow communication between departments.

6. **Switching Architecture:**  
   - Multilayer switches perform both routing and switching.
   - Trunk ports are configured between multilayer switches and 2960 model switches.
   - Access ports are configured between 2960 switches and end-devices.

7. **IP Address Management:**  
   - All devices obtain their IP addresses dynamically from a **DHCP server** located in the server room.
   - Devices in the server room have **static IP addresses**.

8. **Routing Protocol:**  
   - **OSPF** (Open Shortest Path First) is used for routing between routers and multilayer switches.
   - OSPF ensures efficient route advertisement and redundancy.

9. **Network Address Translation:**  
   - **NAT** is configured on the core router to enable internet access for internal devices.

10. **Additional Services:**  
    - **DNS server** provides name resolution for all devices.
    - **Security** is ensured via VLAN segmentation, WPA2 wireless authentication, and static IP allocation for critical systems.

---

## 🖼️ Topology

![Topology](assets/topology.png)

---

## Implementation Details

- **OSPF** is used as the routing protocol on all routers and multilayer switches.
- **NAT** is implemented on the core router for outside connectivity.
- **Inter-VLAN Routing** is set up on multilayer switches for internal communication.
- **DHCP server** automatically provides IP addresses to all devices except those in the server room (which use static IPs).
- **DNS server** is configured for all devices.
- **Trunk ports** are set up for switch-to-switch connections; **access ports** are set for end-device connections.
- **Wireless access point** configured for high device capacity and security.
- **VLANs** established for each department, ensuring traffic isolation and management.
- **Redundancy** and **scalability** considered in design.

---

## 📄 Documentation

**For more information about the project, detailed configuration steps, and design rationale, please check the [Project Report](report.pdf).**

---

## Author

**Adar Sönmez**  
[GitHub Profile](https://github.com/adarSonmez)

---
