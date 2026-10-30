# Kali Linux Networking Commands

## 1. Introduction

This document contains useful Linux commands for inspecting and testing the Kali Linux network configuration.

## 2. IP Address Information

### Display network interfaces and IP addresses

```bash
ip addr
```

### Display IP addresses only

```bash
hostname -I
```

## 3. Routing Information

### Display the routing table

```bash
ip route
```

This command helps identify the default gateway and available network routes.

## 4. NetworkManager Commands

### Display network device status

```bash
nmcli device status
```

### Display available network connections

```bash
nmcli connection show
```

### Display active connections

```bash
nmcli connection show --active
```

## 5. Connectivity Testing

### Test the NAT Network gateway

```bash
ping -c 4 10.0.0.1
```

### Test internet connectivity using an IP address

```bash
ping -c 4 8.8.8.8
```

### Test DNS resolution

```bash
nslookup example.com
```

## 6. Network Troubleshooting

### Restart NetworkManager

```bash
sudo systemctl restart NetworkManager
```

### Check NetworkManager status

```bash
systemctl status NetworkManager
```

## 7. Command Summary

| Command | Purpose |
|---|---|
| `ip addr` | Display network interfaces and IP addresses |
| `hostname -I` | Display assigned IP addresses |
| `ip route` | Display routing information |
| `nmcli device status` | Display network device status |
| `nmcli connection show` | Display saved connections |
| `ping` | Test network connectivity |
| `nslookup` | Test DNS resolution |
| `systemctl status NetworkManager` | Check NetworkManager status |

## 8. Notes

Commands should be executed in the Kali Linux terminal. Record the actual command output and any errors encountered during the lab.
