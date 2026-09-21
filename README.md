Week 3 – Network Security Assessment

Overview : 

This project presents the Week 3 Advanced Cybersecurity Practical Task completed in an authorized virtual laboratory environment.

The assessment focuses on network discovery, Nmap-based security assessment, Wireshark traffic analysis, vulnerability assessment, and security hardening.

Objectives : 

- Perform network discovery using Nmap.
- Identify open ports and services on the authorized Windows 7 test VM.
- Perform service/version and operating system detection.
- Analyze network traffic using Wireshark.
- Correlate Nmap scanning activity with captured network packets.
- Identify potential security weaknesses and vulnerabilities.
- Apply at least three security hardening measures.
- Compare the system before and after hardening.
- Document findings and security recommendations.

Lab Environment : 

| Component | Details |
|---|---|
| Security Testing Machine | Kali Linux |
| Kali IP Address | 10.0.2.4 |
| Target Machine | Windows 7 |
| Windows 7 IP Address | 10.0.2.3 |
| Network | 10.0.2.0/24 |
| Gateway | 10.0.2.1 |
| Virtualization | VirtualBox |

Tools Used : 

- Kali Linux
- Nmap
- Wireshark
- VirtualBox
- Windows Firewall
- diagrams.net

Tasks Completed :

Task 7 – Network Discovery and Basic Nmap
- Identified the lab network configuration.
- Discovered active hosts using Nmap.
- Performed basic port scanning on the Windows 7 VM.

Task 8 – Advanced Nmap Security Assessment
Performed:
- Service and version detection
- Operating system detection
- TCP SYN scanning
- UDP scanning
- Vulnerability assessment using Nmap NSE scripts

Task 9 – Wireshark Network Traffic Analysis
Analyzed:
- DNS
- TCP
- ICMP
- ARP
- UDP traffic

Task 10 – Nmap + Wireshark Investigation
Correlated Nmap SYN scanning activity with Wireshark packets, including TCP SYN, SYN/ACK and RST traffic.

Task 11 – Advanced Network Traffic Investigation
Investigated DNS, TCP, ICMP, ARP, SYN and RST traffic and documented interesting network events.

Task 12 – Vulnerability Assessment
Identified exposed services and potential security weaknesses in the authorized Windows 7 test VM.

Task 13 – Security Hardening
Three firewall-based hardening measures were implemented :
1. Blocked TCP port 445.
2. Blocked TCP port 139.
3. Blocked TCP ports 49152–49158.

Follow-up Nmap scans showed the affected ports as filtered.

Task 14 – Final Security Assessment
The system was assessed before and after hardening to evaluate the reduction in network exposure.

Key Findings :

- SMB service was exposed on TCP port 445.
- NetBIOS service was exposed on TCP port 139.
- Dynamic RPC ports 49152–49158 were exposed before hardening.
- Nmap vulnerability assessment reported a potential MS17-010-related SMB vulnerability.
- Wireshark analysis showed normal DNS, TCP, ICMP and ARP traffic within the authorized lab.

Hardening Results :

| Port(s) | Before | After |
|---|---|---|
| TCP 445 | Open | Filtered |
| TCP 139 | Open | Filtered |
| TCP 49152–49158 | Open | Filtered |

Recommendations :

- Keep Windows Firewall enabled.
- Restrict unnecessary inbound ports.
- Reduce unnecessary SMB and NetBIOS exposure.
- Keep the operating system and security updates current.
- Monitor network traffic for unusual activity.
- Perform regular authorized security assessments.

Authorization and Scope :

All scanning, traffic capture, vulnerability assessment, and hardening activities were performed only against the authorized Windows 7 virtual machine within the controlled VirtualBox laboratory environment.

Conclusion :

This project provided practical experience in network reconnaissance, service enumeration, traffic analysis, vulnerability assessment, and defensive security hardening using Nmap, Wireshark, and Windows Firewall.
