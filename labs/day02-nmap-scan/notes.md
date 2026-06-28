# Day 02: Nmap SYN + Version Scan

**Target:** Metasploitable2 VM @ 192.168.56.102
**Date:** 2026-07-28
**Objective:** Recon with nmap -sS and -sV

### Commands Run
```bash
nmap -sS 192.168.56.102
nmap -sV 192.168.56.102
### Key Findings
- **21/tcp open | ftp | vsftpd 2.3.4** 
    - Note: Known vulnerable version with backdoor. High priority for exploitation later.
- **22/tcp open | ssh | OpenSSH 4.7p1** 
    - Note: Older SSH version. Check for weak credentials/brute force in future labs.
- **80/tcp open | http | Apache httpd 2.2.8** 
    - Note: Web server running. Will scan for directories and vulns in Day 3+.
- **139/tcp, 445/tcp open | smb | Samba 3.0.20** 
    - Note: File sharing service. Common Red Team attack surface.

**Summary:** Metasploitable2 has 5+ open services. All are intentionally vulnerable. FTP 21 is the most exposed.
