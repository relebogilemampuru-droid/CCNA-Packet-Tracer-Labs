# Network Security: Access Control List (ACL) Labs

## 📌 Project Overview
This repository documents a series of comprehensive labs focused on the design, configuration, and validation of **Access Control Lists (ACLs)**. The goal of these labs is to demonstrate technical proficiency in securing network traffic, managing bandwidth, and implementing "Least Privilege" access models within a Cisco-based infrastructure.

## 🛠️ Technologies & Tools
*   **Environment:** Cisco Packet Tracer / GNS3
*   **Hardware Emulation:** Cisco 2900 Series Routers, 2960 Switches
*   **Protocols:** IPv4, TCP/UDP, ICMP, OSPF
*   **Security:** Standard & Extended ACLs, Named & Numbered Lists

## 🚀 Lab Scenarios

### 1. Standard ACL Implementation
*   **Task:** Restrict access to the Server Farm VLAN.
*   **Configuration:** Applied filtering based on source IP addresses to permit only authorized Management workstations while denying all other LAN traffic.
*   **Key Learning:** Optimal placement (closest to the destination).

### 2. Extended ACL & Application Filtering
*   **Task:** Granular traffic control for a multi-departmental network.
*   **Configuration:** 
    *   Permit **HTTP/HTTPS** (Port 80/443) and **DNS** (Port 53).
    *   Deny **FTP** (Port 21) and **ICMP** (Ping) across subnets.
*   **Key Learning:** Filtering based on protocol, source, destination, and port numbers.

### 3. Securing Administrative Access (VTY Lines)
*   **Task:** Harden network devices against unauthorized remote access.
*   **Configuration:** Created an ACL to restrict **SSH** access to specific administrator IP addresses and applied it to `line vty 0 15` using the `access-class` command.

## 🔍 Verification & Troubleshooting
To ensure the integrity of the security policies, the following commands were used to validate the logic:
*   `show access-lists` — To verify match counts and entry order.
*   `show ip interface` — To confirm which ACL is applied to which interface and in what direction (In/Out).
*   **Ping/Telnet/Web Browser Tests:** Practical end-to-end testing to confirm the "Implicit Deny" is functioning as expected.

## 📂 Repository Structure
```text
├── Topologies/           # PDF and Image exports of network diagrams
├── Packet-Tracer-Labs/   # .pkt files for each lab scenario
├── Scripts/              # CLI configuration snippets (Running-Config)
└── Documentation/        # Step-by-step logic and subnetting breakdowns
