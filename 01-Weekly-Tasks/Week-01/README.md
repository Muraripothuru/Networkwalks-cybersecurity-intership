# Week 01 – VirtualBox and Kali Linux Lab Setup

## 1. Introduction

During Week 01 of my cybersecurity internship, I worked on preparing a virtual cybersecurity lab environment using Oracle VM VirtualBox and Kali Linux.

The purpose of this lab is to establish a controlled environment for learning Linux, networking, and cybersecurity tools.

## 2. Objectives

- Prepare the existing VirtualBox environment.
- Configure a NAT Network in VirtualBox.
- Connect the Kali Linux virtual machine to the NAT Network.
- Configure and verify Kali Linux network settings.
- Test network connectivity.
- Configure shared folders and VirtualBox integration features.
- Create a virtual machine snapshot after successful setup.

## 3. Lab Environment

| Component | Configuration |
|---|---|
| Host OS | Windows 11 |
| Virtualization Software | Oracle VM VirtualBox 7.x |
| Guest OS | Kali Linux 2026.1 |
| Network Mode | NAT Network |
| NAT Network Name | NatNetwork |
| IPv4 Prefix | 10.0.0.0/24 |
| DHCP | Enabled |
| IPv6 | Disabled |

*Note: The final Kali IP address, gateway, and DNS will be documented after verification.*

## 4. Lab Activities

### Task 1 – VirtualBox Configuration
Prepared the existing VirtualBox installation and Kali Linux virtual machine.

### Task 2 – NAT Network Configuration
Created a NAT Network named `NatNetwork` with the IPv4 prefix `10.0.0.0/24`. DHCP was enabled and IPv6 was disabled.

### Task 3 – Kali Linux Network Configuration
Configured the Kali Linux virtual machine to use the `NatNetwork` adapter. Further verification of the adapter settings and network connection is required.

### Task 4 – Network Connectivity Testing
Planned to use Linux networking commands to check the IP address, default route, DNS resolution, and connectivity.

### Task 5 – Shared Folder Configuration
Planned to configure a shared folder between the Windows host and Kali Linux guest.

### Task 6 – Virtual Machine Snapshot
A snapshot will be created after the lab environment is fully configured and verified.

## 5. Repository Contents

- `Lab-Setup/` – Configuration documentation.
- `Screenshots/` – Evidence of the lab setup and verification.
- `Notes/` – Commands, troubleshooting steps, and learning notes.

## 6. Learning Outcomes

Through this lab, I aim to understand:

- Virtualization and virtual machine configuration.
- NAT Network configuration.
- Kali Linux network management.
- Basic network troubleshooting.
- Connectivity and DNS verification.
- The importance of virtual machine snapshots.

## 7. Current Status

**Status: In Progress**

The NAT Network has been created. Remaining configuration and verification tasks will be updated as they are completed.

## 8. Safety and Ethics

All cybersecurity activities will be performed only in authorized lab environments and for educational purposes.
