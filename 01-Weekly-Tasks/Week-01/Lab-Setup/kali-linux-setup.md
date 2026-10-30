# Kali Linux Setup

## 1. Overview

This document describes the preparation of the existing Kali Linux virtual machine for the cybersecurity internship lab.

Kali Linux is a Linux distribution commonly used for cybersecurity learning, penetration testing, security assessment, and digital forensics.

## 2. Environment Details

| Component | Details |
|---|---|
| Guest Operating System | Kali Linux 2026.1 |
| Virtualization Software | Oracle VM VirtualBox 7.x |
| Host Operating System | Windows 11 |
| Network | NatNetwork |

## 3. Virtual Machine Preparation

The existing Kali Linux virtual machine was used.

Preparation activities:

1. Open Oracle VM VirtualBox.
2. Select the existing Kali Linux virtual machine.
3. Review the virtual machine settings.
4. Check the network adapter configuration.
5. Start Kali Linux.
6. Log in to the Kali Linux desktop.

## 4. Accessing Network Settings

Network settings can be accessed through the Kali Linux desktop:

1. Open the network icon in the top-right panel.
2. Select the connection settings or Edit Connections option.
3. Select the wired network connection.
4. Open its settings.
5. Navigate to the IPv4 Settings section.

Alternatively, open a terminal and run:

```bash
nm-connection-editor
```

## 5. Network Information

Use these commands to inspect the network configuration:

```bash
ip addr
ip route
nmcli
```

The actual IP address, gateway, and DNS information should be recorded after checking the command output.

## 6. Shared Folder Integration

A Windows Downloads folder is planned to be shared with Kali Linux through VirtualBox.

The intended shared folder name is:

`Downloads`

The shared folder will be verified after configuration.

## 7. Conclusion

The existing Kali Linux virtual machine is being prepared for the internship lab. Network configuration and shared folder integration remain subject to verification.
