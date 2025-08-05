 🌐 Internship Project: Port Scanning & Network Analysis


This repository contains my cybersecurity internship task, which involves analyzing network ports, researching common services, and evaluating potential security risks using tools like Nmap and Wireshark.


---


## 📁 Files Included

File Name                                             Description

combinedscanresults.txt                               Raw output of multiple Nmap scans conducted on different IPs in the network.

nmap_captureusingwireshark(only 1 case).pcapng        Wireshark capture file showing Nmap SYN scan packets.

research_common_ports_and_risk.md                     Notes or research about ports, services, and potential vulnerabilities.

commands_nmap.png                                     Screenshot showing various Nmap commands used during the scan.
  
wireshark_capture_analysis.png                        Screenshot of Wireshark with highlighted SYN packets for analysis.
🧪 Tools Used

    Nmap: For port scanning and service detection.
    Wireshark: For capturing and analyzing packet-level data.
    Linux (Kali): Operating system used for conducting scans and analysis.

🔍 Tasks Completed
1. Common Services Running on Open Ports

Based on the Nmap output, the following services were identified:

    53/tcp: DNS (dnsmasq)
    135/tcp: MS RPC
    445/tcp: SMB (Microsoft DS)
    80/tcp: HTTP (Google Web Server)
    443/tcp: HTTPS (Google Web Server)

2. Security Risks from Open Ports

    Port 53: May allow DNS cache poisoning or amplification attacks.
    Port 135: Vulnerable to RPC-based attacks like MS08-067.
    Port 445: Often targeted by SMB vulnerabilities like EternalBlue.
    Port 80: Transmits data unencrypted, susceptible to MITM attacks.
    Port 443: More secure but can be misconfigured with weak TLS versions.

🖥️ Wireshark Observations
The Wireshark capture file shows SYN packets from 10.0.2.17 scanning multiple ports on other IPs. This is typical behavior for an Nmap TCP SYN ("stealth") scan. Reset responses and filtered ports are also visible

Screenshots
1 NMAP commands screenshots.
2 Wireshark capture screenshot.


📌 Summary

This analysis helped me understand how to:

    Perform detailed port scans using Nmap.
    Analyze and interpret packet-level data in Wireshark.
    Research service-specific vulnerabilities.
