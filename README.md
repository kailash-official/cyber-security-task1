# Cyber Security Task 1

## Network Scanning and Reconnaissance

### Objective
To identify active hosts, open ports, services, and operating system information using Nmap and Zenmap.

### Tools Used
- Nmap
- Zenmap

### Target IP
192.168.56.1

### Scan Results

| Port | Service | Status |
|--------|---------|---------|
| 135 | MSRPC | Open |
| 139 | NetBIOS | Open |
| 445 | Microsoft-DS (SMB) | Open |

### Findings
- The target host was active.
- Open ports 135, 139, and 445 were detected.
- Microsoft Windows services were identified.
- SMB file-sharing services were running.

### Conclusion
The network scan successfully identified active services and open ports on the target system.
