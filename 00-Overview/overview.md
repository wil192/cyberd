# Project Overview

## Table of Contents

- [Project Purpose](#project-purpose)
- [Scope](#scope)
- [Architecture Summary](#architecture-summary)
- [Key Components](#key-components)
- [Goals and Objectives](#goals-and-objectives)
- [Glossary](#glossary)

---

## Project Purpose

This project simulates an enterprise environment with organizational, attack, and defense entities for cybersecurity training and testing.

---

## Scope

- Virtualized infrastructure using Proxmox VE.
- Network segmentation using VLANs and firewalls.
- Multiple VMs representing different entities.
- Simulated attack and defense scenarios.
- Comprehensive documentation and playbooks.

---

## Architecture Summary

- Proxmox VE cluster hosts all virtual machines.
- pfSense appliance manages network segmentation, firewalling, and routing.
- Entities divided into organizational, attack, and defense groups.
- Networks designed for isolation and controlled communication.

---

## Key Components

- **Proxmox VE**: Virtualization platform.
- **pfSense**: Network appliance and firewall.
- **VMs**: Various virtual machines simulating roles.
- **Networks**: VLANs, bridges, and firewall rules.

---

## Goals and Objectives

- Create realistic cyber ranges.
- Facilitate training for attack and defense.
- Maintain reproducible and manageable environment.
- Provide clear documentation and playbooks.

---

## Glossary

- **VM**: Virtual Machine  
- **VLAN**: Virtual Local Area Network  
- **Proxmox VE**: Proxmox Virtual Environment  
- **pfSense**: Open source firewall/router software  
- **Entity**: A logical group like organization, attack, defense

