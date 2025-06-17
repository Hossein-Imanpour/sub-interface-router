# 🚦 Inter-VLAN Routing using Sub-Interfaces (Router-on-a-Stick)

## 📘 Project Overview
This project demonstrates communication between three VLANs using sub-interfaces configured on a single router interface. The method used is known as **Router-on-a-Stick**, which is a fundamental concept in CCNA and is commonly used in small to mid-sized networks.

## 🧱 Topology Description
Three VLANs are configured to represent different departments within an organization. A Layer 2 switch connects end devices to the router, which handles inter-VLAN routing via sub-interfaces over a trunk link.

## 🧩 VLAN & IP Details

| VLAN    | Subnet            | Device IPs                | Sub-Interface     |
|---------|-------------------|---------------------------|-------------------|
| VLAN 10 | 192.168.1.0/24    | 192.168.1.10, .11         | `Gig0/1.10`       |
| VLAN 20 | 192.168.20.0/24   | 192.168.20.10             | `Gig0/2.20`       |
| VLAN 30 | 192.168.30.0/24   | 192.168.30.10             | `Gig0/3.30`       |

> 📝 Note: Each sub-interface on the router is assigned an IP address within its respective subnet and uses IEEE 802.1Q encapsulation for VLAN tagging.

## 🧪 Testing & Verification

- [x] Successful ping between hosts across VLANs
- [x] Correct subnetting and IP addressing
- [x] VLANs defined and assigned to switch ports
- [x] Trunk connection between switch and router operational

## 🖼 Network Diagram
> A visual topology screenshot is included as `topology.png` (if available).

## ⚙️ Tools Used
- Cisco Packet Tracer
- Cisco Router with sub-interfaces
- Layer 2 Switch
- Static IP configuration on hosts

## 💡 Learning Objectives
- Understanding Access vs Trunk Ports
- Configuring router sub-interfaces using `encapsulation dot1q`
- Limitations of Router-on-a-Stick in large networks

---

### ✅ Suggestions for Future Enhancements

- Add a DHCP server instead of static IP addressing
- Use a Layer 3 switch for direct inter-VLAN routing
- Add DNS or Web servers to simulate real-world services