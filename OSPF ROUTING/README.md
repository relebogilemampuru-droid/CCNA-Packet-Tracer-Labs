# 🛣️ Lab: Multi-Area OSPF Dynamic Routing

### Objective
To implement a scalable and efficient routing architecture using **Open Shortest Path First (OSPFv2)**. This lab demonstrates the ability to manage complex routing tables and ensure fast network convergence.

### Key Configurations:
* **Area Hierarchy:** Established a Backbone Area (Area 0) and Area 1 to demonstrate hierarchical routing logic.
* **DR/BDR Election:** Manually assigned Router IDs and priorities to ensure predictable Designated Router elections.
* **Passive Interfaces:** Secured LAN-facing ports using `passive-interface` to stop unnecessary OSPF Hello packets.
* **Metric Tuning:** Adjusted interface bandwidth and cost to manipulate path selection for optimal traffic flow.

### Verification Commands:
* `show ip ospf neighbor` – Verified "FULL" adjacency states between all routers.
* `show ip route ospf` – Confirmed the presence of Inter-area (O IA) and Intra-area (O) routes.
* `show ip ospf interface brief` – Checked OSPF process IDs and area assignments across interfaces.
