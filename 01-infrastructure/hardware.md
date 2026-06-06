# Hardware

[← Infrastructure ](./README.md)

This page documents the physical hardware used in my home lab environment.

## Hardware Inventory

| Device | Role |
|----------|----------|
| ZTE T5400 | Router |
| Lenovo ThinkPad L480 | Proxmox Host |
| Lenovo ThinkPad E16 Gen 1 | Workstation |

## SOHO Router – ZTE T5400

* **LAN Network:** 192.168.254.0/24
* **Wi-Fi:** Disabled
* **DHCP:** Disabled
* **Firewall:** Deny all incoming connections
* **Embedded Switch:** 4 × 1 Gbps RJ45 ports

### Purpose

Provides internet connectivity and basic network routing for the lab environment. DHCP and Wi-Fi services are disabled to allow infrastructure services to be managed by dedicated virtual servers.

## Lenovo ThinkPad L480

* **CPU:** Intel Core i5-8250U
* **RAM:** 24 GB DDR4-2400
* **Storage:**
  * 512 GB External SATA SSD
  * 2 TB External HDD
* **Network Interface:** 1 Gbps Ethernet

### Purpose

Dedicated Proxmox VE host used to run:
* Windows servers
* Linux servers

## Lenovo ThinkPad E16 Gen 1

* **CPU:** Intel Core i5-1335U
* **RAM:** 16 GB DDR4-3200
* **Storage:**
  * 512 GB M.2 SSD
  
### Purpose

Personal workstation running Hyper-V to host simulated end-user workstations integrated with Active Directory for testing and administration purposes.