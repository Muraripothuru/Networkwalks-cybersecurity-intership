# Week 01 – Lab Environment Setup

## 1. Overview

This week focuses on preparing a virtual cybersecurity lab environment using Oracle VM VirtualBox and Kali Linux.

The objective is to create a controlled environment for learning and performing authorized cybersecurity practical exercises.

## 2. Objectives

- Prepare the virtual lab environment.
- Configure the VirtualBox NAT Network.
- Configure the Kali Linux network connection.
- Verify network connectivity.
- Take a snapshot of the virtual machine after setup.

## 3. Lab Environment

| Component | Configuration |
|---|---|
| Host Operating System | Windows 11 |
| Virtualization Software | Oracle VM VirtualBox 7.x |
| Guest Operating System | Kali Linux 2026.1 |
| Network Mode | NAT Network |
| NAT Network Name | NatNetwork |
| Network Subnet | 10.0.0.0/24 |
| DHCP | Enabled |

*Note: Record the final Kali IP address, gateway, and DNS only after verifying them in Kali Linux.*

## 4. Lab Tasks

### Task 1 – VirtualBox Preparation
- Checked the existing VirtualBox installation.
- Prepared the existing Kali Linux virtual machine.

### Task 2 – NAT Network Configuration
- Created a NAT Network named `NatNetwork`.
- Configured the IPv4 prefix as `10.0.0.0/24`.
- Enabled DHCP.
- Disabled IPv6.

### Task 3 – Kali Linux Network Configuration
- Connected the Kali Linux virtual machine to `NatNetwork`.
- Checked the virtual network adapter settings.
- Pending: verify the final network configuration and resolve any VirtualBox configuration warnings.

### Task 4 – Network Connectivity Verification
Commands to use:

```bash
ip addr
ip route
nmcli
ping -c 4 10.0.0.1
ping -c 4 8.8.8.8
nslookup google.com
```

*Record the actual output and results after running these commands.*

### Task 5 – Shared Folder and Integration
- Pending: configure the Windows shared folder.
- Pending: verify clipboard and drag-and-drop integration, if supported.
- Pending: verify Guest Additions if required.

### Task 6 – Virtual Machine Snapshot
- Pending: take a snapshot after completing and verifying the lab configuration.

## 5. Screenshots

Add screenshots as evidence of your work:

- VirtualBox NAT Network configuration.
- Kali Linux network adapter settings.
- Kali Linux IP configuration.
- Network connectivity test results.
- Shared folder configuration.
- Virtual machine snapshot.

## 6. Issues and Troubleshooting

Document any errors encountered during setup and the steps taken to resolve them.

## 7. Learning Outcomes

By completing this lab, I aim to understand:

- Virtual machine configuration using VirtualBox.
- NAT Network configuration.
- Basic Kali Linux network management.
- Network connectivity verification.
- The importance of snapshots and a controlled lab environment.

## 8. Status

**In Progress**

Tasks will be marked complete only after configuration and verification.

## 9. Safety and Ethics

All cybersecurity activities in this internship lab will be performed only in authorized environments and for educational purposes.
