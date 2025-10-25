# Experiment 7 – RIP Routing Topology

## 🧩 Overview
This experiment simulates a three-router topology using RIP v2 for dynamic routing.

## 🖥️ Devices Used
- 3 Routers (PT-Router)
- 3 Switches (2960)
- 6 PCs

## 🌐 IP Addressing
| Device     | Interface        | IP Address      | Subnet Mask       |
|------------|------------------|------------------|-------------------|
| Router0    | Fa0/0            | 192.168.10.1     | 255.255.255.0     |
| Router0    | Serial2/0 (DCE)  | 10.0.0.1         | 255.255.255.252   |
| PC0        | NIC              | 192.168.10.2     | 255.255.255.0     |
| ...        | ...              | ...              | ...               |

## 🔧 Routing Protocol
```bash
router rip
version 2
network 192.168.10.0
network 10.0.0.0
