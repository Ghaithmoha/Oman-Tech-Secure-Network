# 🏢 Oman Tech: Secure Network Infrastructure

## 📌 Project Overview
This repository contains the design, configuration, and implementation of a secure enterprise network infrastructure for "Oman Tech". The project transitions the organization from a vulnerable flat network to a highly secure, segmented architecture using physical isolation and strict Least-Privilege policies.

## 🛠️ Technologies & Features Implemented
* **Subnet Segmentation:** Network divided into discrete `/24` subnets for Finance, HR, IT, Management, and Server Farm.
* **Access Control Lists (ACLs):** Extended ACLs enforced on the core routing level to strictly isolate inter-departmental traffic (e.g., blocking HR from Finance).
* **Perimeter Security (Firewall):** Cisco ASA 5506-X deployment with dynamic NAT (PAT) and stateful packet inspection.
* **Core Services:** Centralized DHCP Relay (`ip helper-address`) and DNS server configurations.
* **Layer-2 Security:** Switch port hardening and Sticky MAC Port-Security.

## 🖧 Hardware Used (Cisco Packet Tracer 8.2)
* **Core Router:** Cisco 2811 (equipped with NM-4E expansion module for physical segmentation).
* **Edge Firewall:** Cisco ASA 5506-X.
* **Access Layer:** Cisco Catalyst 2960-24TT Switches.
* **End Devices:** Generic PCs & Centralized Enterprise Server.

## 📁 Repository Contents
1. `Oman_Tech_Network_vFinal.pkt`: The complete Cisco Packet Tracer simulation file.
2. `/Configurations`: Directory containing the full CLI scripts for the Core Router, ASA Firewall, and Access Switches.
3. `Network_Topology.png`: Visual representation of the implemented architecture.

## 🚀 How to Run
1. Download and install **Cisco Packet Tracer 8.2** (or newer).
2. Clone this repository or download the `.pkt` file.
3. Open the simulation and utilize the CLI terminals to review the `show access-lists` and `show ip interface brief` commands.
