<div align="center">
  <h1>🧠 Network Administration: Real-World GNS3 Lab</h1>
  <h3>🔧 VLANs, IP Routing, ACLs, NAT, and Interdepartmental Network Segmentation</h3>
</div>

## 📁 Project Overview

This project simulates a real-world corporate network for "Phoenix Corp" using GNS3. It includes VLAN configuration, IP addressing, switch and router setup, NAT, ACLs, and inter-VLAN routing for departments: HR, IT, and Sales.

---

## 🖥️ Network Topology

- **3 Departments**: HR (Green), IT (Light Green), Sales (Blue)
- **2 Layer 2 Switches** connecting all PCs
- **Router for Inter-VLAN routing and NAT**
- **12 VPCS Nodes** distributed equally across departments

---

## 🧩 Network Design Summary

| Department | VLAN Tag | Subnet | VPCS Assigned |
|------------|----------|--------|----------------|
| HR         | 10       | 192.168.2.0/24 | PC1–PC4 |
| IT         | 20       | 192.168.1.0/24 | PC5–PC8 |
| Sales      | 30       | 192.168.3.0/24 | PC9–PC12 |

Switches and ports are configured per VLAN, and inter-switch trunking is set up on port 12.

---

## 🔧 Key Configuration Steps

### 🛠️ Switch Configuration
- VLANs created and assigned (tags 10, 20, 30)
- Ports mapped to appropriate VLANs
- Trunk link established between switches

### 🌐 IP Addressing
Each PC manually configured with appropriate IP address.

### 🌍 Inter-VLAN Routing
- Router configured with interfaces for each VLAN
- Gateway addresses set for all PCs
- Routing and NAT enabled

### 🔒 Access Control Lists
- Permit/deny traffic between departments
- Specific source/destination ACLs implemented

---

## 🧪 Testing & Verification

✅ Successful Pings within same VLAN  
❌ Inter-VLAN ping blocked (until routing enabled)  
✅ ACL applied to selectively allow/block traffic  
✅ NAT rules configured and verified  
✅ Wireshark used for ARP & ICMP packet capture  
✅ DNS resolution and traceroutes for external domains (`amazon.com`, `twitter.com`, `youtube.com`)

---

## 📸 Screenshots

<img src="images/topology.png" width="700" />
<img src="images/vlan-config.png" width="700" />

---

## 📚 Tools Used
- **GNS3**
- **VyOS Router**
- **ExtremeXOS Switches**
- **VPCS**
- **Wireshark**

---

## ✅ Project Status
**Completed** – Network segmented by departments, routed, and secured with ACLs and NAT.

---

## 🧠 Lessons Learned
- VLAN and switch port mapping
- Inter-VLAN routing configuration
- Creating and applying ACLs
- Real-world simulation of enterprise networking scenarios

