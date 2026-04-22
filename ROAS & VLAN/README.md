# 🚀 Lab: Inter-VLAN Routing (Router-on-a-Stick) & Segmentation

### Objective
To implement a scalable Inter-VLAN routing solution using a single physical interface (ROAS) and to enforce network segmentation across multiple departments.

### Key Configurations:
* **802.1Q Encapsulation:** Configured logical sub-interfaces on the ISR 4331 routers to handle tagged traffic from multiple VLANs.
* **VLAN Segmentation:** Created and named departmental VLANs (Sales, Marketing, Engineering, HR) to isolate broadcast domains.
* **Trunking & Access Ports:** Established IEEE 802.1Q trunks between switches and routers while locking down end-user access ports.
* **DHCP Automation:** Deployed localized DHCP pools for each sub-interface to ensure seamless IP assignment across logical boundaries.

### Verification Commands:
* `show ip interface brief` – Verified sub-interface status and IP assignments.
* `show vlan brief` – Confirmed VLAN database consistency across switches.
* `show interfaces trunk` – Ensured 802.1Q tags are correctly traversing the uplinks.
* `show ip route` – Validated that the router is correctly identifying and routing between the logical subnets.

This lab highlights my ability to maximize hardware efficiency by using logical sub-interfaces to bridge multiple networks, a critical skill for managing modern, secure enterprise environments.
