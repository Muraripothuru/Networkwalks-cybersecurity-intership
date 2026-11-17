
# PM1 – Footprinting and Reconnaissance

## Objective

The objective of PM1 was to perform authorised footprinting and reconnaissance of the `networkwalks.com` domain using different information-gathering tools available in Kali Linux.

## Target Information

- Target domain: `networkwalks.com`
- Operating environment: Kali Linux
- Activity: Information gathering and reconnaissance
- Scope: Authorised internship testing

## Tools Used

| Tool | Purpose |
|---|---|
| WHOIS | Domain registration lookup |
| WhatWeb | Website technology fingerprinting |
| Nslookup | DNS resolution |
| cURL | HTTP header inspection |
| WAFW00F | Web Application Firewall identification |
| DNSRecon | DNS enumeration |

## Activities Performed

1. WHOIS lookup to examine public domain registration information.
2. WhatWeb scan to identify web technology indicators.
3. Nslookup to retrieve domain and name-server information.
4. cURL to inspect HTTP response headers.
5. WAFW00F to identify possible WAF protection.
6. DNSRecon to collect DNS records.

## Results

The tools provided information about domain registration, web server indicators, HTTP responses, DNS infrastructure and reported WAF technology.

Detailed findings are available in [Findings.md](./Findings.md).

## Screenshots

| Screenshot | Description |
|---|---|
| 01-whois.png | WHOIS lookup |
| 02-whatweb.png | WhatWeb output |
| 03-nslookup.png | DNS lookup |
| 04-curl.png | HTTP headers |
| 05-wafw00f.png | WAF identification |
| 06-dnsrecon.png | DNS enumeration |

## Conclusion

PM1 provided practical experience in using different reconnaissance tools to collect and interpret publicly available domain and web information.

All findings should be interpreted as observations, not confirmed vulnerabilities.

