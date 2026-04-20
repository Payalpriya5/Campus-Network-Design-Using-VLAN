# 🌐 Campus Network Topology – Cisco Packet Tracer

A multi-department campus network simulation built using **Cisco Packet Tracer**, featuring inter-VLAN routing, a multilayer switch core, and three distinct departmental segments connected to the internet via a router and cloud.

---

## 📸 Network Diagram

![Network Topology](./1776667356330_image.png)

---

## 🏗️ Network Overview

This project simulates a campus-level LAN with three departments, a core multilayer switch, an edge router, and cloud connectivity.

| Component | Device | Role |
|---|---|---|
| Cloud | Cloud-PT (Cloud0) | Internet/WAN simulation |
| Edge Router | Cisco 2911 (Router0) | Gateway to cloud |
| Core Switch | Cisco 3560-24PS (Multilayer Switch0) | Inter-VLAN routing & core switching |
| CSE Dept Switch | Cisco 2960-24TT (Switch0) | Access layer – CSE |
| Admin Dept Switch | Cisco 2960-24TT (Switch1) | Access layer – Admin |
| Library Switch | Cisco 2960-24TT (Switch2) | Access layer – Library |

---

## 🏢 Departments

### 💻 CSE_DEPT
- **Switch:** Switch0 (2960-24TT)
- **End Devices:** PC0, PC1, PC2, Printer0

### 🏛️ ADMIN_DEPT
- **Switch:** Switch1 (2960-24TT)
- **End Devices:** PC3, PC4, PC5, Server0

### 📚 LIBRARY
- **Switch:** Switch2 (2960-24TT)
- **End Devices:** PC6, PC7, Laptop0

---

## 🔗 Topology Summary

```
Cloud0
  └── Router0 (2911)
        └── Multilayer Switch0 (3560-24PS)   ← Core / Inter-VLAN Router
              ├── Switch0 (CSE_DEPT)
              │     ├── PC0
              │     ├── PC1
              │     ├── PC2
              │     └── Printer0
              ├── Switch1 (ADMIN_DEPT)
              │     ├── PC3
              │     ├── PC4
              │     ├── PC5
              │     └── Server0
              └── Switch2 (LIBRARY)
                    ├── PC6
                    ├── PC7
                    └── Laptop0
```

---

## 🛠️ Technologies Used

- **Cisco Packet Tracer** – Network simulation
- **Cisco 2911 Router** – Edge routing
- **Cisco 3560-24PS Multilayer Switch** – Layer 3 switching / Inter-VLAN routing
- **Cisco 2960-24TT Switches** – Layer 2 access switches
- **VLANs** – Department segmentation
- **Cloud-PT** – Simulated internet/WAN

---

## 🚀 Getting Started

1. Install [Cisco Packet Tracer](https://www.netacad.com/courses/packet-tracer) (free with a NetAcad account).
2. Clone this repository:
   ```bash
   git clone https://github.com/your-username/your-repo-name.git
   ```
3. Open the `.pkt` file in Cisco Packet Tracer.
4. Explore the topology, ping between devices, and inspect switch/router configurations.

---

## 📋 Features

- ✅ Three VLANs (one per department)
- ✅ Inter-VLAN routing via multilayer switch
- ✅ Internet connectivity through Cloud-PT
- ✅ Server and printer integration
- ✅ Wired and wireless (laptop) end devices

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).

---

## 🙋 Author

> Built as part of a computer networking course/lab project.  
> Feel free to fork, modify, and learn from it!
