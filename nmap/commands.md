# SCAN TECHNIQUE

| Command | Example                | Description                             |
| ------- | ---------------------- | --------------------------------------- |
| `-sS`   | `nmap -sS 192.168.1.1` | Stealthy SYN scan (default, needs root) |
| `-sT`   | `nmap -sT 192.168.1.1` | TCP connect scan (non-root users)       |
| `-sU`   | `nmap -sU 192.168.1.1` | UDP scan                                |

# HOST DISCOVERY

| Command | Example                   | Description                         |
| ------- | ------------------------- | ----------------------------------- |
| `-sn`   | `nmap -sn 192.168.1.0/24` | Ping scan for live hosts            |
| `-Pn`   | `nmap -Pn 192.168.1.1`    | Skip host discovery (assume online) |
| `-PR`   | `nmap -PR 192.168.1.0/24` | ARP discovery (local LAN)           |

# PORT SPECIFICATION
| Command       | Example                             | Description                   |
| ------------- | ----------------------------------- | ----------------------------- |
| `-p`          | `nmap -p 22,80 192.168.1.1`         | Scan specific ports           |
| `-p-`         | `nmap -p- 192.168.1.1`              | Scan all 65535 ports          |
| `-F`          | `nmap -F 192.168.1.1`               | Fast scan of top 100 ports    |
| `--top-ports` | `nmap --top-ports 1000 192.168.1.1` | Scan top x ports by frequency |

# OS DETECTION
| Command | Example               | Description                                     |
| ------- | --------------------- | ----------------------------------------------- |
| `-O`    | `nmap -O 192.168.1.1` | Detect OS via TCP/IP fingerprinting             |
| `-A`    | `nmap -A 192.168.1.1` | Detect OS + services + script scan + traceroute |

# TIMING AND PERFORMANCE
| Command | Example                | Description                      |
| ------- | ---------------------- | -------------------------------- |
| `-T1`   | `nmap -T1 192.168.1.1` | Slow, stealthy scan              |
| `-T3`   | `nmap -T3 192.168.1.1` | Normal speed (default)           |
| `-T4`   | `nmap -T4 192.168.1.1` | Faster scans for stable networks |
