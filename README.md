
# AfyaCare Clinic Network – Packet Tracer Lab

This project is a realistic small-enterprise network simulation for a fictional healthcare clinic (AfyaCare), built in Cisco Packet Tracer.

The goal of this lab is to practice **real-world networking fundamentals**:
- VLAN design
- Inter-VLAN routing on multilayer switches
- Basic router configuration
- Branch office connectivity
- Secure device management with SSH
- Basic network hardening

This is an educational lab, not a production-ready design.

---
 Topology Overview

- HQ:
  - 1 Edge Router (R1)
  - 2 Multilayer Switches (DSW1, DSW2)
  - 1 Access Switch (ASW1)
- Branch:
  - 1 Router (BR1)
  - 1 Access Switch
- End Devices:
  - User PCs
  - Server
  - CCTV device
  - Management PC

---

IP Addressing & VLANs

| VLAN | Purpose     | Subnet         | Gateway        |
|------|-------------|----------------|----------------|
| 10   | Users       | 10.10.10.0/24  | 10.10.10.1     |
| 30   | CCTV        | 10.10.30.0/24  | 10.10.30.1     |
| 40   | Servers     | 10.10.40.0/24  | 10.10.40.1     |
| 99   | Management  | 10.10.99.0/24  | 10.10.99.1     |
| —    | Branch LAN  | 10.20.10.0/24  | 10.20.10.1     |

---

 Features Implemented

- VLAN segmentation for security and performance
- Inter-VLAN routing on multilayer switches
- Static routing between HQ and branch
- SSH-only device management
- Basic device hardening (no DNS lookup, encrypted passwords)
- Trunking between switches

---

How to Use

1. Download and install Cisco Packet Tracer.
2. Clone this repository:
   ```bash

   git clone https://github.com/your-username/afycare-packet-tracer-lab.git

