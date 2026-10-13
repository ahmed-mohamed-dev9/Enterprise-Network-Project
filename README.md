# 🌐 Enterprise Multi-Site Network Infrastructure Design & Implementation

An enterprise-grade WAN/LAN network topology designed, configured, and verified using **Cisco Packet Tracer**. This project simulates a mid-sized organization with 7 interconnecting sites, featuring redundant routing, Layer 2 security, and automated services.

---

## 📐 Key Network Features & Technologies
* **Dynamic Routing:** OSPFv2 (Process 1000, Area 0) configured across 8 Cisco ISR 4331 routers.
* **First-Hop Redundancy:** HSRP (Group 1) active/standby setup between R2 and R8 for Site 2 high availability.
* **Inter-VLAN Routing:** Router-on-a-Stick (802.1Q sub-interfaces) on R5 for IT (VLAN 100) and Engineering (VLAN 200).
* **Link Aggregation:** 2-port LACP EtherChannel (Port-channel 1) between switches S8 and S9.
* **Security & Access Control:**
  * Extended ACLs on R4 restricting traffic to Web/FTP/ICMP services.
  * Standard VTY ACLs & SSH-only remote management on R2.
  * Layer 2 hardening (Port Security, Sticky MAC, PortFast, BPDU Guard) on access switch S1.
* **Network Services:** Static NAT publishing an internal web server (200.10.15.20), centralized DHCP, and authoritative NTP synchronization.

---

## 📑 Detailed Documentation & Implementation Report
For full IP addressing plans, command-by-command explanations, and verification tests, refer to the uploaded PDF report: **Enterprise_Multi_Site_Network_Report2.pdf**.

---

## 💻 How to Run the Project
1. Download and install **Cisco Packet Tracer**.
2. Download the `.pkt` file from this repository.
3. Open `Final Project CCNA 200-301#13and last.pkt` in Packet Tracer to inspect or test the topology.
