# Network Configuration

## 1. Overview

This document records the NAT Network configuration and Kali Linux network setup for the Week 01 cybersecurity lab.

The purpose is to provide network connectivity to the Kali Linux virtual machine through VirtualBox.

## 2. NAT Network Configuration

The following NAT Network was created in VirtualBox:

| Setting | Value |
|---|---|
| Network Name | NatNetwork |
| IPv4 Prefix | 10.0.0.0/24 |
| DHCP | Enabled |
| IPv6 | Disabled |

## 3. Kali Linux Network Adapter

The Kali Linux virtual machine was configured with:

| Setting | Value |
|---|---|
| Adapter | Adapter 1 |
| Attached To | NAT Network |
| Network Name | NatNetwork |
| Adapter Type | Intel PRO/1000 MT Desktop (82540EM) |
| Promiscuous Mode | Allow All |
| Cable Connected | Enabled |

A VirtualBox invalid-settings warning was observed and requires investigation.

## 4. Kali Linux IP Configuration

The following commands can be used to inspect network settings:

```bash
ip addr
ip route
nmcli device status
nmcli connection show
```

Record the verified values below:

| Network Parameter | Actual Value |
|---|---|
| Kali IPv4 Address | Pending verification |
| Subnet Mask / Prefix | Pending verification |
| Default Gateway | Pending verification |
| DNS Server | Pending verification |

Do not assume that an intended IP address or gateway has been configured until it is confirmed in Kali Linux.

## 5. Connectivity Testing

Run the following commands:

```bash
ping -c 4 10.0.0.1
ping -c 4 8.8.8.8
nslookup example.com
```

Record the results:

| Test | Result |
|---|---|
| Gateway connectivity | Pending |
| Internet connectivity by IP | Pending |
| DNS resolution | Pending |

## 6. Troubleshooting

If connectivity fails:

- Check whether the VirtualBox network adapter is enabled.
- Confirm that the VM is connected to `NatNetwork`.
- Check the Kali Linux IP address.
- Inspect the default route.
- Check DNS configuration.
- Review the VirtualBox invalid-settings warning.

## 7. Conclusion

The NAT Network has been created successfully. Kali Linux network configuration and connectivity tests still need to be verified.
