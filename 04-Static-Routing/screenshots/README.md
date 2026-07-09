# 🌐 Static Routing using Cisco Packet Tracer

This project demonstrates the implementation of **Static Routing** between two different Local Area Networks (LANs) using **Cisco Packet Tracer**.

Static Routing is a manual routing method where routes are configured by the network administrator. In this lab, two separate networks communicate successfully through two routers using static routes.

---

# 📌 Project Overview

In this lab, I:

- Designed a network consisting of two LANs.
- Configured IP addresses on routers and PCs.
- Connected two routers using a point-to-point network.
- Configured Static Routes on both routers.
- Verified routing tables and interface status.
- Successfully tested end-to-end connectivity using Ping.

---

# 🖥️ Network Topology

The network consists of:

- 2 Cisco 2911 Routers
- 2 Cisco 2960-24TT Switches
- 2 PCs

## Topology Diagram

![Network Topology](screenshots/topology.png)

---

# 🌍 IP Addressing Scheme

| Device | Interface | IP Address | Subnet Mask |
|---------|-----------|------------|-------------|
| PC0 | FastEthernet0 | 192.168.1.10 | 255.255.255.0 |
| Router0 | GigabitEthernet0/0 | 192.168.1.1 | 255.255.255.0 |
| Router0 | GigabitEthernet0/1 | 10.0.0.1 | 255.255.255.252 |
| Router1 | GigabitEthernet0/1 | 10.0.0.2 | 255.255.255.252 |
| Router1 | GigabitEthernet0/0 | 192.168.2.1 | 255.255.255.0 |
| PC1 | FastEthernet0 | 192.168.2.10 | 255.255.255.0 |

---

# ⚙️ Configuration Summary

### Router0

- Configured GigabitEthernet0/0 for LAN 1.
- Configured GigabitEthernet0/1 for Router-to-Router communication.
- Added a Static Route to reach Network **192.168.2.0/24**.

### Router1

- Configured GigabitEthernet0/0 for LAN 2.
- Configured GigabitEthernet0/1 for Router-to-Router communication.
- Added a Static Route to reach Network **192.168.1.0/24**.

---

# ✅ Verification Commands

The following Cisco IOS commands were used to verify the configuration:

```bash
show ip interface brief

show ip route

show running-config
```

Connectivity was verified using:

```bash
ping 192.168.2.10
```

---

# 📷 Screenshots

## 🖥️ Network Topology

![Network Topology](screenshots/topology.png)

---

## ⚙️ Router0 Configuration

![Router0 Configuration](screenshots/router0-config.png)

---

## ⚙️ Router1 Configuration

![Router1 Configuration](screenshots/router1-config.png)

---

## 📡 Router0 Interface Status

![Router0 Interface Status](screenshots/show-ip-interface-brief-router0.png)

---

## 📡 Router1 Interface Status

![Router1 Interface Status](screenshots/show-ip-interface-brief-router1.png)

---

## 🛣️ Router0 Routing Table

![Router0 Routing Table](screenshots/show-ip-route-router0.png)

---

## 🛣️ Router1 Routing Table

![Router1 Routing Table](screenshots/show-ip-route-router1.png)

---

## ✅ End-to-End Connectivity Test

Successful communication between **PC0 (192.168.1.10)** and **PC1 (192.168.2.10)** using Static Routing.

![Ping Test](screenshots/ping-test.png)

---

# 🎯 Learning Outcomes

After completing this lab, I learned:

- Static Routing Fundamentals
- Router Interface Configuration
- IP Address Assignment
- Point-to-Point Router Communication
- Manual Route Configuration
- Routing Table Verification
- Network Connectivity Testing
- Network Troubleshooting using Cisco IOS commands

---

# 🛠️ Tools Used

- Cisco Packet Tracer
- Cisco IOS CLI
- Git & GitHub

---

# 💡 Key Concepts

- Static Routing
- Router-to-Router Communication
- IPv4 Addressing
- Routing Tables
- Next-Hop Routing
- End-to-End Connectivity
- Network Troubleshooting

---

# 👩‍💻 Author

**Prachi Jogdand**

🎓 BE Graduate in Computer Science & Engineering (Artificial Intelligence & Machine Learning)

🔐 Aspiring Network Engineer | Cybersecurity Enthusiast
