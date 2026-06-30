
## Day 4: Nmap NSE Scripts on Metasploitable 2

**Objective**: Move from service mapping to vulnerability identification using NSE.

**Target**: Metasploitable 2 @ 192.168.56.102  
**Attacker**: Kali Linux @ 192.168.56.101

**Command Run:**
```bash
nmap -sV --script vuln 192.168.56.102
