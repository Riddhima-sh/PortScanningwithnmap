# PortScanningwithnmap
This is a basic project which will expand upon the linux command "nmap" which is mainly used for port scanning.

# What is a Port?
A port is a communication endpoint where data is exchanged between a device and the internet or another device. Each port has a number and works with an IP address to handle internet traffic. Ports are managed via:

TCP (Transmission Control Protocol): Reliable, connection-oriented.

UDP (User Datagram Protocol): Fast, connectionless, and often used for streaming.

| Port     | Protocol                     | 
| -------- | -----------------------------|
| 20 (UDP) | FTP Data Transfer            |
| 22 (TCP) | SSH - Secure Logins          |
| 23 (TCP) | Telnet - Unencrypted         |
| 53 (UDP) | DNS - Domain Name Resolution |
| 80 (TCP) | HTTP - Web Browsing          |


# Port Scanning 
Port scanning is a technique used to discover open ports and services on a system. It helps identify vulnerabilities and check for misconfigured or insecure systems.

# Purpose:

-> Determine active services

-> Identify ports receiving/sending data

-> Assess security device presence (e.g., firewalls)

-> Detect login and authentication behaviors

# Port Scanning Techniques
| Technique           | Description                                                                             |
| ------------------- | --------------------------------------------------------------------------------------- |
| **Ping Scan**       | Sends ICMP requests to check if systems are up.                                         |
| **Vanilla Scan**    | Attempts full TCP connections on all ports; easily detected.                            |
| **SYN Scan**        | "Half-open" scan — sends SYN, waits for SYN-ACK, never completes connection (stealthy). |
| **XMAS Scan**       | Sends a packet with multiple flags set — reveals firewall rules and port states.        |
| **FIN Scan**        | Sends a FIN flag — used to probe ports without opening a full session.                  |
| **FTP Bounce Scan** | Disguises origin by relaying through an FTP server.                                     |
| **Sweep Scan**      | Sends packets to a single port across multiple hosts to discover active machines.       |


# Nmap

Nmap (Network Mapper) is a powerful, open-source tool used for:

-> Network discovery

-> Security auditing

-> Host/service detection

-> OS and version detection

-> Firewall and packet filtering analysis

# Features:

Nmap is ...

-> Flexible: Supports advanced scanning methods and evasion techniques.

-> Powerful: Can scan networks with thousands of hosts.

-> Portable: Works on Linux, Windows, macOS, BSD, etc.

-> User-Friendly: CLI (nmap) and GUI (Zenmap) interfaces.

-> Free & Open Source: Comes with full source code and liberal licensing.

-> Well-Documented: Backed by official documentation, books, tutorials, and a strong community

# Nmap Suite Includes:
-> Nmap: Command-line scanner

-> Zenmap: GUI frontend

-> Ncat: Network data transfer tool

-> Ndiff: Compare scan results

-> Nping: Packet generation & response analysis

# Project Overview
Port scanning is a crucial step in network reconnaissance. This script utilizes nmap to:

-> Identify open, closed, and filtered ports

-> Detect services running on those ports

-> Perform OS detection and version detection

-> Generate organized scan reports

# Tools Used 
Nmap: Network scanning utility for port discovery and security auditing.

Python (optional): For wrapping and automating scans.

Linux Terminal / Bash Script: Used for direct Nmap commands.

# Conclusion
-> Use of basic and advanced nmap scan types

-> Syntax and flags for customizing scans

-> Ethical use of scanning tools for vulnerability assessment 

-> Output parsing and logging scan results

# Learning Resources
https://nmap.org/book/man.html


