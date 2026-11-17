# Zenmap Network Scanning – Findings

## 1. Objective

The objective of this activity was to perform network scanning using Zenmap, the graphical interface for Nmap, to identify active hosts and discover open TCP ports on the authorized target.

## 2. Target Information

- **Target Domain:** networkwalks.com
- **Resolved IP Address:** 192.232.216.135
- **Tool Used:** Zenmap / Nmap
- **Nmap Version:** 7.991
- **Scan Type:** SYN Stealth Scan
- **Ports Scanned:** Default 1,000 TCP ports

## 3. Scan Results

The scan successfully resolved the target domain to IP address `192.232.216.135` and identified the host during the ping scan.

The following open TCP ports were discovered:

| Port | Protocol | Common Service |
|---|---|---|
| 21 | TCP | FTP |
| 22 | TCP | SSH |
| 53 | TCP | DNS |
| 80 | TCP | HTTP |
| 110 | TCP | POP3 |
| 143 | TCP | IMAP |
| 443 | TCP | HTTPS |
| 587 | TCP | SMTP Submission |
| 993 | TCP | IMAPS |
| 995 | TCP | POP3S |
| 2222 | TCP | Alternative SSH |

**Total open ports reported: 11**

Note: The service names above are commonly associated with these port numbers. The supplied scan output does not include service-version detection, so the actual services running on these ports have not been independently confirmed.

## 4. Observations

The scan identified several ports commonly associated with web hosting, remote administration, DNS, and email services.

- Ports 80 and 443 are commonly used for HTTP and HTTPS web traffic.
- Ports 21 and 22 are commonly associated with FTP and SSH access.
- Port 53 is commonly associated with DNS services.
- Ports 110, 143, 993, and 995 are commonly associated with email retrieval.
- Port 587 is commonly used for email submission.
- Port 2222 may provide an alternative remote-access service.

The scan also reported dropped probes, increased transmission delays, and retransmission-limit warnings. These messages indicate that some scan probes did not receive timely responses, which may affect scan completeness.

## 5. Troubleshooting and Limitations

During the scan, Nmap displayed multiple timing-related warnings, including dropped probes and retransmission-limit messages. The scan adjusted its sending delay automatically to handle these conditions.

Although 11 open ports were identified, the output does not establish the exact software versions or confirm the services operating on each port. Further authorized service detection would be required for that level of detail.

## 6. Conclusion

The Zenmap scanning activity demonstrated how Nmap can be used to identify a target host and discover open TCP ports. The scan identified 11 open ports on the resolved IP address `192.232.216.135`.

This activity provided practical experience in network reconnaissance, port discovery, interpreting scan output, and understanding the importance of scan limitations when evaluating results.

All findings should be considered preliminary and interpreted within the scope of the authorized assessment.
