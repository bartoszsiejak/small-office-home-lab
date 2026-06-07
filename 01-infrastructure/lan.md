# LAN

[← Infrastructure ](./README.md)

This page describes my lab's LAN.

## IP Adressing
* **IPv6:** Disabled
* **Network:** 192.168.254.0
* **Subnet:** 255.255.255.0
* **Gateway:** 192.168.254.1
* **Static IP:** for servers only

### Physical Devices

| Device | IP Address | Role |
|----------|----------|----------|
| ZTE T5400 | 192.168.254.1 | Router |
| Lenovo ThinkPad L480 | 192.168.254.2 | Proxmox Host |
| Lenovo ThinkPad E16 | 192.168.254.254 | Hyper-V Host |

### Virtual Machines

| VM | IP Address | Role |
|----------|----------|----------|
| WINSERV-01 | 192.168.254.10 | Active Directory Domain Controller, File Server, DHCP, DNS |
| WIN11-01 | DHCP Assigned | Simulated User Workstation |

### Containers

| VM | IP Address | Role |
|----------|----------|----------|
| UBUNTU-01 | 192.168.254.20 | Apache Server |

## DHCP

* **DHCP scope:** 192.168.254.50 - 192.168.254.99
* **DHCP reservation:** Not configured (planned for network printers)

## DNS

* **Domain name:** siejak.local
* **DNS server IP address:** 192.168.254.10
* **DNS forwarding addresses:** 
    * 8.8.8.8 
    * 8.8.4.4

## Network Services

Services running in LAN:
* DNS
* DHCP
* File Sharing
* Active Directory
* Apache Web Server