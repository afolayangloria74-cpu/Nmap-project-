# Nmap-project-lab-scan
For Cybersecurity 
# 🔍 Nmap Lab Project - Network Discovery & Security Auditing

> By AFOLAYAN GLORIA MARVELOUS | IT Support Intern | FUOYE

## Overview
Hands-on lab using Nmap for port scanning in controlled private lab. Part of my cybersecurity learning after Cisco Introduction to Cybersecurity cert.

## Objectives
- Perform SYN stealth scan
- Identify open ports and services
- Understand attack surface

## Tools Used
- Nmap 7.94
- Kali Linux / Windows Terminal
- Wireshark

## Commands

```bash
nmap -sS 192.168.XX.XX


RESULTS
135/tcp open msrpc
139/tcp open netbios-ssn
445/tcp open microsoft-ds
5357/tcp open wsdapi
Nmap done: 1 IP in 0.84s

nmap -sV 192.168.XX.XX
nmap --script vuln 192.168.XX.XX
## Security Analysis

Port 135 - msrpc - Medium risk - Ensure RPC filtering enabled

Port 139 - netbios-ssn - High risk - Disable NetBIOS if not needed, it's old protocol

Port 445 - microsoft-ds (SMB) - High risk - Disable SMBv1 and restrict SMB access, ransomware uses it

Port 5357 - wsdapi - Low risk - Disable if not using network discovery

Key Insight: 996 ports closed means good security. Less open ports = safer.

## What I Learned
1. SYN scan is stealthier than normal scan
2. Every open port can be hacked
3. Windows default services need to be secured
4. Always get permission before scanning - I scanned only my own lab

## Ethical Disclaimer
This scan was performed ONLY on my personal lab device (192.168.XX.XX - private network). Never scan networks you don't own. Unauthorized scanning is illegal.

## Future Improvements
- Add version detection
- Run vulnerability scripts
- Create network map
- Write firewall rules

## About Me
AFOLAYAN GLORIA MARVELOUS
IT Support Intern at Semester Technologies (2 years)
BSc Software Engineering, FUOYE
Cisco Certified - Introduction to Cybersecurity
Skills: Networking, TCP/IP, Wireshark, Linux, IT Support

LinkedIn: linkedin.com/in/afolayan-gloria-b613b642b
Open to Entry-Level Cybersecurity Roles

## License
For educational purposes only.

---
Star this repo and connect with me on LinkedIn!
