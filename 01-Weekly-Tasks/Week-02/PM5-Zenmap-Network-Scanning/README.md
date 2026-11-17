
# PM5 – Network Scanning Using Nmap and Zenmap

## Objective

The objective of PM5 is to understand network discovery and port scanning using Nmap and its graphical interface, Zenmap.

## Lab Environment

| Component | Configuration |
|---|---|
| Host OS | Windows 11 |
| Virtual Machine | Kali Linux |
| Virtualisation | Oracle VirtualBox |
| Kali NAT interface | eth0 |
| Kali Host-only interface | eth1 |
| Kali Host-only IP | 192.168.56.101 |
| Windows Host-only IP | 192.168.56.1 |
| Network | 192.168.56.0/24 |

## Network Configuration

Kali Linux was configured with:

- Adapter 1: NAT for internet connectivity.
- Adapter 2: Host-only Adapter for isolated testing.

The college Wi-Fi network was not used as a scan target.

## Host Discovery

Command:

`sudo nmap -4 -sn -n -e eth1 192.168.56.1`

Nmap successfully identified the Windows host-only adapter as active.

Detailed results are documented in [Findings.md](./Findings.md).

## Zenmap Port Scanning

Recorded the actual Zenmap scan profile, command, port results and screenshots after completing the scan.

Do not report ports or services as open unless the scan confirms them.

## Screenshots

- 01-zenmap-scan.png
- 02-zenmap-ports-hosts.png
- 03-zenmap-topology.png

## Ethical Considerations

All scanning is restricted to the isolated VirtualBox lab and authorised systems. Shared college networks are excluded from the test scope.

