# Network Topology

## Table of Contents

- [Overview](#overview)
- [Physical Network Layout](#physical-network-layout)
- [Virtual Network Components](#virtual-network-components)
- [VLAN Assignments](#vlan-assignments)
- [Bridges and Interfaces](#bridges-and-interfaces)
- [Routing and Firewalling](#routing-and-firewalling)
- [Diagram](#diagram)

---

## Overview

This document describes the network design for the cyber simulation environment.

---

## Physical Network Layout

- Single physical host running Proxmox VE.
- Network interfaces:
  - `eno1`: Primary uplink
  - `eno2`: Management network or backup
- Physical switch supports VLAN tagging.

---

## Virtual Network Components

- Bridges (`vmbr0`, `vmbr1`, etc.) created on Proxmox.
- VLAN interfaces to segment traffic.
- pfSense VM with multiple NICs to route and firewall VLANs.

---

## VLAN Assignments

| VLAN ID | Name          | Purpose               |
|---------|---------------|-----------------------|
| 10      | Org_Network   | Organizational VMs    |
| 20      | Attack_Network| Attack infrastructure |
| 30      | Defense_Network| Defense infrastructure|

---

## Bridges and Interfaces

- `vmbr0` - Bridge connected to physical interface `eno1`, tagged for VLAN 10.
- `vmbr1` - Bridge for VLAN 20 traffic.
- `vmbr2` - Bridge for VLAN 30 traffic.

---

## Routing and Firewalling

- pfSense routes between VLANs as required.
- Firewall rules restrict traffic flow according to security policy.
- NAT applied for external internet access.

---

## Diagram

*(Insert your network diagram here. Could be a link to an image or a Mermaid.js diagram if supported.)*

