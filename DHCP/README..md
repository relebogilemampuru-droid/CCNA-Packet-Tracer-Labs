# 🌐 Lab: Automated IP Management with DHCP

### Objective
To implement a reliable and automated IP addressing scheme, reducing manual configuration errors and ensuring seamless network access for end-user devices.

### Key Configurations:
* **Exclusion Lists:** Reserved static IP addresses for critical infrastructure (Default Gateways, Servers, and Printers) using `ip dhcp excluded-address`.
* **Pool Customization:** Defined network ranges, default routers, and DNS server details for different VLANs.
* **Lease Management:** Configured optimal lease times to balance network stability with address availability.
* **DHCP Relay (Helper Address):** Implemented `ip helper-address` on multi-layer switches to allow DHCP requests to cross broadcast domains.

### Verification Commands:
* `show ip dhcp binding` – Confirmed active IP assignments to client MAC addresses.
* `show ip dhcp pool` – Monitored address utilization and available scope.
* `show ip dhcp server statistics` – Verified the DORA (Discover, Offer, Request, Acknowledge) process.

### Professional Mentality
> "Automation is not about replacing the engineer; it's about freeing the engineer to solve bigger problems."

Efficient IP management is the first step toward a scalable enterprise. This lab demonstrates my ability to manage local resources while maintaining the strict address control required for a secure environment.
