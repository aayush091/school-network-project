## 📘 School Network Project

Designed and implemented a multi-branch enterprise network connecting Darwin (core site), Tennant Creek, and Alice Springs. The project integrates multiple routing protocols, centralized services, redundancy mechanisms, and security controls to ensure reliable and scalable network communication.

---

## 🌐 Network Overview

- **Darwin (Main Site)**  
  - Core network using EIGRP  
  - Hosts centralized services (DNS, DHCP, HTTP)  
  - Implements HSRP for gateway redundancy  

- **Tennant Creek (Branch)**  
  - OSPF Area 0  
  - VLAN segmentation with DHCP relay  

- **Alice Springs (Branch)**  
  - OSPF Area 1  
  - Redundant switching using EtherChannel  
  - STP optimization for load balancing  

- **Interconnection**  
  - WAN links using /30 subnetting  
  - Route redistribution between EIGRP and OSPF  

---

## 🔧 Technologies & Concepts

- EIGRP (core routing)
- OSPF (multi-area design)
- Route Redistribution
- VLAN & Inter-VLAN Routing (ROAS)
- HSRP (gateway redundancy)
- DHCP (centralized + relay)
- DNS (name resolution across branches)
- HTTP (web server hosting – *school.com*)
- ACL (traffic control and security)
- EtherChannel & STP (Layer 2 redundancy)

---

## 🔐 Security Implementation

Access Control Lists (ACLs) were configured to regulate traffic flow within the network.

- Student VLAN traffic is restricted to only required services  
- Web server access (HTTP/HTTPS) is permitted  
- Unnecessary or unauthorized communication is blocked  

This ensures controlled and secure access to centralized resources.

---

## 🧪 Testing & Verification

- ✔ End-to-end connectivity verified using `ping`
- ✔ Routing tables confirmed across all routers
- ✔ DNS resolution tested using domain name (*school.com*)
- ✔ Web server accessed from all branches via browser
- ✔ DHCP successfully assigns IP addresses dynamically
- ✔ ACL behavior validated (restricted and permitted traffic)

---

## ⚠️ Challenges & Solutions

- Incorrect subnet masks preventing gateway communication  
- HSRP duplicate IP conflicts due to misconfigured virtual IP  
- DHCP failure due to incorrect `ip helper-address` placement  
- DNS resolution issues across branches (resolved via record replication)  
- OSPF adjacency issues due to incorrect area configuration  
- ACL misconfiguration due to rule order and syntax errors  

All issues were resolved through systematic troubleshooting and verification.

---

## 📸 Network Screenshots

### Darwin Main Network
darwin_main.png

### Alice Springs Branch
Alice Spring.png

### Tennant Creek Branch
TennantCREEK.png)

---

## 📂 Project Files

- 📄 `report/` → Full project documentation  
- 🌐 `topology/` → Packet Tracer (.pkt) file  
- 🖼 `screenshots/` → Network and configuration visuals  

---

## 🎯 Key Outcome

This project demonstrates the ability to design, configure, troubleshoot, and secure a multi-site enterprise network using industry-relevant technologies and best practices.

---

## 👤 Author

**Aayush Dhakal**  
🔗 LinkedIn: www.linkedin.com/in/aayush-dhakal-526107315  
