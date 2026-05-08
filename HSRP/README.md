# 🚀 HSRP & Gateway Redundancy Labs

## 📌 Project Overview
This repository contains a collection of **Cisco Packet Tracer** labs focused on implementing **First Hop Redundancy Protocols (FHRP)**, specifically **HSRP (Hot Standby Router Protocol)**. 

The goal of these labs is to demonstrate the configuration and management of high-availability networks where "zero downtime" is the priority. By sharing a virtual IP address between multiple multilayer switches or routers, these topologies ensure that if a primary gateway fails, the backup takes over seamlessly without interrupting the end-user experience.

---

## 🛠️ Technical Features Implemented
* **HSRP Configuration:** Setting up Active/Standby states with custom priorities and preemption.
* **DHCP Integration:** Configuring centralized DHCP pools on multilayer switches to automate IP assignment for client workstations.
* **VLAN Segmentation:** Using 802.1Q trunking to manage traffic across Access and Distribution layers.
* **Failover Testing:** Documented scenarios where links are manually disabled to verify sub-second convergence and packet path redirection.
* **Inter-VLAN Routing:** Implementing Switch Virtual Interfaces (SVIs) to allow communication between different departments/VLANs.

---

## 📐 Topology Architecture
The labs follow a **Hierarchical Network Design**:
1. **Core/Distribution Layer:** Two Cisco 3560 Multilayer Switches acting as the HSRP pair.
2. **Access Layer:** Cisco 2960 Switches connecting end-devices.
3. **End Devices:** PCs configured for dynamic addressing via the HSRP Virtual Gateway.

---

## 💻 Key Commands Used
### HSRP Verification
```bash
show standby brief
show standby
