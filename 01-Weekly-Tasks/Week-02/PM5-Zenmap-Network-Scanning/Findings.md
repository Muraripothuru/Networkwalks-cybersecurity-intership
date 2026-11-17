
# PM5 – Network Scanning Findings

## 1. VirtualBox Network Setup

A Host-only Adapter was configured as the second network interface for Kali Linux.

Kali Linux:

- eth0: `10.0.2.15/24`
- eth1: `192.168.56.101/24`

Windows host-only adapter:

- IPv4: `192.168.56.1`
- Subnet mask: `255.255.255.0`

## 2. Host Discovery

**Command:**

`sudo nmap -4 -sn -n -e eth1 192.168.56.1`

**Actual result:**

- Target: `192.168.56.1`
- Host status: Up
- Latency: Approximately `0.00050s`
- MAC address: `0A:00:27:00:00:03`
- Scan type: Host discovery
- Network interface: `eth1`

The scan successfully identified the Windows host-only adapter.

## 3. Connectivity Observation

An ICMP ping test did not receive replies. However, Nmap host discovery successfully identified the host as active.

This demonstrates that a failed ping does not necessarily mean a system is offline.

## 4. Zenmap Port Scan

**Status: Complete this section after the actual Zenmap scan.**

- Zenmap profile: [Enter actual profile]
- Scan command: [Enter actual command]
- Open ports: [Enter actual results]
- Closed ports: [Enter actual results]
- Filtered ports: [Enter actual results]
- Services identified: [Enter actual results]

Attach the actual Zenmap screenshots.

## 5. Conclusion

The isolated VirtualBox network was configured successfully, and Nmap host discovery identified the Windows host-only adapter.

The final port-scanning findings must be added after completing the Zenmap scan.

