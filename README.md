<div align="center">
<h1># 🏢 Enterprise Network Infrastructure: A Real-World VLAN and Routing Lab</h1>
</div>

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
> 🔽 **Screenshots:**
<img src="https://github.com/InfoSec01/Network-Administration/blob/main/Topology%20-%20Installing%20and%20Configuring%20Routers.png" width="70%"/>
<img src="https://github.com/InfoSec01/Network-Administration/blob/main/Topology%20-%20Designing%20Implementing%20Logical%20Networks%20.png" width="70%"/>
<img src="https://github.com/InfoSec01/Network-Administration/blob/main/Topology%20-%20Analyzing%20Troubleshooting%20Network%20Traffic%20Connectivity.png" width="70%"/>

## 🖼️ Wireshark Capture and IP Forwarding
> 🔽 **Screenshots:**
<img src="https://github.com/InfoSec01/Network-Administration/blob/main/hr-it-forwarding-vlan.png" width="60%"/>
<img src="https://github.com/InfoSec01/Network-Administration/blob/main/icpm-capture-wireshark.png" width="60%"/>
<img src="https://github.com/InfoSec01/Network-Administration/blob/main/arp-capture-wireshark.png" width="60%"/>

## 🚀 Let’s Work Together

I bring not only technical ability, but a deep understanding of operational impact. I continue to learn building systems that work—securely, efficiently, and resiliently.

📬 **Contact me**
- baratulkhan@gmail.com

---
