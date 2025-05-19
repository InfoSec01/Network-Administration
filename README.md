# 🏢 Enterprise Network Infrastructure: A Real-World VLAN and Routing Lab

> **"Designing networks isn't just about connectivity — it's about accountability, security, and scaling with confidence."**

Welcome to a hands-on project that mirrors the demands of a real-world enterprise network. This lab was engineered not for certification, but for **production-grade readiness** — simulating how companies protect, segment, and manage their internal network environments using VLANs, ACLs, inter-VLAN routing, and NAT.  

Built entirely in **GNS3**, this is more than a lab — it's a **proof-of-skill**.

---

## 🚀 Project Overview

**Objective:**  
To build and secure a multi-department enterprise network, ensuring:
- Segmentation between departments  
- Controlled access and communication  
- Internet simulation with NAT and DNS testing  
- Troubleshooting capabilities for real-world issues  

**Simulated Company Departments:**  
- 📁 **Human Resources (HR)**  
- 🖥️ **Information Technology (IT)**  
- 📦 **Sales**

---

## 🧩 Architecture at a Glance

- 🧑‍💻 **12 VPCS Hosts** – 4 per department  
- 🧠 **2 Extreme EXOS Switches** – VLANs, Trunks, ACLs  
- 🌐 **VyOS Router** – Inter-VLAN Routing, NAT, Gateway  
- 🧪 **Wireshark Integration** – Live traffic analysis  
- ⚙️ **Private DNS & Internet Simulation**

---

## 🛠️ Network Design Highlights

### 🔹 VLANs & Trunking
- VLAN 10: HR  
- VLAN 20: IT  
- VLAN 30: Sales  
- Configured on both switches with 802.1Q trunking to ensure seamless VLAN propagation across infrastructure.

### 🔸 Inter-VLAN Routing
- Enabled selectively on VyOS to allow **controlled communication** between departments.  
- ACLs block unauthorized cross-department access.

### 🔐 Access Control Lists (ACLs)
- Enforced on switches to limit traffic between specific VLANs.  
- Simulates **Zero Trust** policies — users access only what they are permitted to.

### 🌍 NAT & DNS
- VyOS performs **Source NAT** so internal hosts can simulate reaching external resources.  
- DNS tests (e.g., `nslookup amazon.com`, `tracert`) validate routing and name resolution.

### 🧰 Troubleshooting & Validation
- Live diagnostics using:
  - `ping`, `tracert`, `ipconfig`, `arp`, `nslookup`  
  - Wireshark captures to analyze real packet flow
- Intentional misconfigurations tested and resolved to reflect real IT operational challenges.

## 🖼️ Network Topology

Here is the network topology of several projects:


---
