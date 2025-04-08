# Corporate Network Design & Configuration – Packet Tracer Project

## Overview

This project simulates a corporate network for **HSBC Bank**, as part of the KV4011 – *Introduction to Networks and Cyber Security* module. The objective is to design, configure, and secure a multi-branch network using **Cisco Packet Tracer**.

## Project Context

HSBC is expanding with three new branches in:
- **Manchester** (130 hosts)
- **Birmingham** (250 hosts)
- **Edinburgh** (220 hosts)

The **Main Office** is based in **Leeds** (70 hosts), which also serves as the central hub connected to the **Internet** and all branches through **point-to-point links**.

---

## Network Design Highlights

- **IPv4 Addressing** using **VLSM** within the `192.x.x.x/22` private range.
- Subnetting designed to meet current and future host requirements.
- Each site is connected via point-to-point links to Leeds (main office).
- The ISP provides `130.175.123.0/30` for internet connectivity.

---

## Hardware Topology

- **4 Cisco Routers**
- **4 Cisco Switches**
- **Multiple End Devices (PCs)** according to branch requirements
- **1 ISP Router**

---

## Configuration Summary

- **Static Routing** for simplicity and predictability
- **SSH access** enabled on all routers
- **Password protection**:
  - Console access
  - VTY (Telnet/SSH) lines
  - Enable secret
- Hostnames and IP addresses configured per device
- Verified using essential show commands:
  - `show ip interface brief`
  - `show running-config`
  - `show ip route`
  - `show version`
  - `show cdp neighbors`

---

## Security Measures Implemented

- SSH-enabled remote access (with RSA keys)
- Secure console and vty access with strong passwords
- Role-based access considered
- Suggested: implementation of **firewalls** and **IDS/IPS** for perimeter defense (documented in the report)

---

## File Contents

- `Network 1.pkt` – Cisco Packet Tracer file representing the full network
- Configuration details included in report appendix

---

## How to Use

1. Open the `.pkt` file using **Cisco Packet Tracer (v8.2 or newer)**.
2. Explore the topology and device configurations.
3. Use `Simulation Mode` to test connectivity between branches and the internet.
4. View security features in router configs (SSH setup, password-protected lines, etc).

---

## Author

**[Daniel Que]**  

---

