# DNS-Sinkhole

## Objective
To configure and deploy our own DNS Sinkhole using BIND9 on a self-hosted Ubuntu VPS. This projects goal is to block access to known malicious domains by redirecting DNS queries to a controlled IP, improving security and visibility over network traffic.

### Skills Learned
- Deployed and configured a DNS server using BIND9 on Ubuntu.
- Implemented DNS redirection for malicious domain blocking.
- Analyzed DNS traffic using Wireshark and dig.
- Managed Linux system services (systemd) and DNS records.
- Performed local DNS override on macOS using network settings.
- Troubleshooted DNS resolution and routing behavior.

### Tools Used
- DigitalOcean (cloud platform for VPS)
- BIND9 (DNS server software)
- Ubuntu Linux (server OS)
- SSH/Secure Shell (remote access to VPS)
- dig/nslookup/Wireshark (for DNS testing and inspection)

## Steps
- Deployed a new Ubuntu VPS via DigitalOcean and connected via SSH.
- Installed and started BIND9 (named) DNS server.
- Configured a zone file to sinkhole badsite.com and pointed it to 0.0.0.0.
- Updated local DNS settings on macOS using networksetup to point to the VPS.
- Verified DNS sinkhole by querying with dig and testing domain access in a browser.
- Used Wireshark to analyze DNS traffic and confirm redirection behavior.
