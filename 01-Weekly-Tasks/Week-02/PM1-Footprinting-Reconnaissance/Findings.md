
# PM1 – Technical Findings

## 1. WHOIS

**Command:**

`whois networkwalks.com`

**Observation:**

The WHOIS lookup was completed successfully. It provided publicly available domain registration information.

Refer to the saved WHOIS screenshot for the exact registrar, registration dates and name-server details.

## 2. WhatWeb

**Command:**

`whatweb --max-threads=1 --open-timeout=5 --read-timeout=10 --no-errors https://networkwalks.com/`

**Observations from captured output:**

- Apache server indicator identified.
- WordPress-related indicators observed.
- HTTP-to-HTTPS redirect observed.
- Cookie named `__wpdm_client` identified.

The scan did not establish a verified software version. No specific version is claimed here.

## 3. Nslookup

**Commands:**

`nslookup networkwalks.com`

`nslookup -type=NS networkwalks.com`

**Observation:**

Both DNS lookup activities were completed. The screenshots contain the exact returned DNS information.

## 4. cURL

**Command:**

`curl -I --connect-timeout 10 --max-time 20 https://networkwalks.com`

**Observations:**

- HTTP response: `200 OK`
- Server header: `Apache`
- WordPress REST API link was present.
- Content type: `text/html; charset=UTF-8`
- Cookie: `__wpdm_client`
- Cookie attributes included `Secure` and `HttpOnly`.
- Referrer-Policy and Permissions-Policy headers were observed.

## 5. WAFW00F

**Command:**

`wafw00f https://networkwalks.com/`

**Result:**

WAFW00F reported:

`The site is behind ModSecurity (SpiderLabs) WAF.`

Number of requests: 2.

This is a tool-based identification result and does not prove the complete effectiveness of the WAF.

## 6. DNSRecon

**Command:**

`dnsrecon -d networkwalks.com`

**Results:**

- SOA: `ns6135.hostgator.com`
- Name server: `ns6135.hostgator.com`
- Additional name server: `ns6136.hostgator.com`
- MX: `mail.networkwalks.com`
- DNS server version string: `9.16.23-RH`
- SPF TXT record identified.
- Google site-verification TXT record identified.
- Autodiscover SRV records identified.
- Total records reported: 8.

DNSSEC query observation:

`No answer for DNSSEC query`

This response alone is not sufficient to establish whether DNSSEC is disabled.

## 7. Conclusion

The PM1 activities demonstrated how different tools can be combined to gather information about domain registration, DNS infrastructure, web technologies, HTTP responses and reported security controls.

The findings are reconnaissance observations and should not be treated as confirmed vulnerabilities.

