# Troubleshooting Notes

## 1. Overview

This document records issues encountered during the Week 01 VirtualBox and Kali Linux lab setup, along with investigation steps and solutions.

## 2. Issue: VirtualBox Invalid Settings Warning

**Description:**

An "Invalid settings detected" warning appeared in the VirtualBox virtual machine network settings.

**Configuration being reviewed:**

- Adapter 1 enabled.
- Attached to NAT Network.
- Network name: `NatNetwork`.
- Adapter type: Intel PRO/1000 MT Desktop (82540EM).
- Promiscuous Mode: Allow All.
- Cable Connected: Enabled.

**Investigation steps:**

1. Open the Kali Linux virtual machine settings.
2. Navigate to Network → Adapter 1.
3. Check that the NAT Network is selected.
4. Inspect the warning details displayed by VirtualBox.
5. Apply the correction based on the exact warning message.

**Status:** Pending investigation.

## 3. Issue: Kali Linux Network Connectivity

**Description:**

Network connectivity needs to be verified after connecting Kali Linux to the NAT Network.

**Investigation commands:**

```bash
ip addr
ip route
nmcli device status
ping -c 4 10.0.0.1
```

**Status:** Pending verification.

## 4. Issue: DNS Resolution

**Description:**

DNS resolution needs to be tested after confirming network connectivity.

**Investigation command:**

```bash
nslookup example.com
```

**Status:** Pending verification.

## 5. Issue: Shared Folder Access

**Description:**

The Windows Downloads folder is planned to be shared with Kali Linux.

**Investigation steps:**

1. Check the VirtualBox shared folder settings.
2. Confirm the shared folder name is `Downloads`.
3. Check whether Guest Additions are installed.
4. Verify that the Kali Linux user has permission to access the shared folder.

**Status:** Pending configuration.

## 6. Troubleshooting Record

| Issue | Investigation | Status |
|---|---|---|
| VirtualBox invalid settings | Inspect warning details | Pending |
| Kali network connectivity | Check IP and route | Pending |
| DNS resolution | Run nslookup | Pending |
| Shared folder access | Check Guest Additions and permissions | Pending |

## 7. Conclusion

This document will be updated as issues are identified, investigated, and resolved during the lab setup.
