# VirtualBox Configuration

## 1. Overview

This document describes the preparation and configuration of Oracle VM VirtualBox for the Week 01 cybersecurity lab.

An existing VirtualBox installation and Kali Linux virtual machine were used instead of reinstalling the software.

## 2. System Environment

| Component | Details |
|---|---|
| Host Operating System | Windows 11 |
| Virtualization Software | Oracle VM VirtualBox 7.x |
| Guest Operating System | Kali Linux 2026.1 |
| Virtual Machine | Existing Kali Linux VM |

## 3. Virtual Machine Preparation

The existing Kali Linux virtual machine was selected for the lab.

The following settings were reviewed:

- Virtual machine name and operating system.
- System memory allocation.
- Processor allocation.
- Network adapter configuration.
- Virtual hard disk availability.

## 4. Network Adapter Configuration

The Kali Linux virtual machine was configured with the following intended settings:

| Setting | Value |
|---|---|
| Adapter | Adapter 1 |
| Enable Network Adapter | Enabled |
| Attached To | NAT Network |
| Network Name | NatNetwork |
| Adapter Type | Intel PRO/1000 MT Desktop (82540EM) |
| Promiscuous Mode | Allow All |
| Cable Connected | Enabled |

**Note:** A VirtualBox warning about invalid settings was observed during configuration. The exact cause must be checked and resolved before considering the configuration complete.

## 5. Verification

After resolving any configuration warnings, verify that:

- The virtual machine starts successfully.
- The network adapter is enabled.
- The correct NAT Network is selected.
- Kali Linux can access the configured network.

## 6. Conclusion

VirtualBox was prepared using the existing installation and Kali Linux virtual machine. Network configuration and verification are ongoing.

## 7. Evidence

Refer to the screenshots stored in the `../Screenshots/` directory.
