
## Day 4: Nmap NSE Scripts on Metasploitable 2

**Objective**: Move from service mapping to vulnerability identification using NSE.

**Target**: Metasploitable 2 @ 192.168.56.102  
**Attacker**: Kali Linux @ 192.168.56.101

**Command Run:**
```bash
nmap -sV --script vuln 192.168.56.102
21/tcp   open  ftp     vsftpd 2.3.4
| ftp-vsftpd-backdoor: 
|   VULNERABLE:
|   vsftpd 2.3.4 backdoor
|       State: VULNERABLE 
|       IDs:  CVE:CVE-2011-2523
