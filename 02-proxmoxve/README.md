# Proxmox Virtual Environment

[← Back To Home](../README.md)

## Overview

This section covers the deployment, configuration, and issues related to Proxmox VE. Proxmox VE is used as the main hypervisor to host virtual machines

## Cluster Configuration

### pve01.siejak.local

#### Hardware 

* **CPU:** Intel Core i5-8250U
* **RAM:** 24 GB DDR4-2400
* **Storage:**
  * 512 GB External SATA SSD
  * 2 TB External HDD
* **Network Interface:** 1 Gbps Ethernet

#### System configuration 
- **Current version:** 9.2.2
- **Kernel version:** 7.0.2-6-pve
- **Boot disk filesystem:** ext4
- **IP address:** 192.168.254.2 (static)
- **DNS server:** 192.168.254.1
- **Gateway:** 192.168.254.1

#### Update sources (only no-subscription)

* http://deb.debian.org/debian/
* http://security.debian.org/debian-security/
* http://download.proxmox.com/debian/pve