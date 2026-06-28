## Day 3 - OS Detection with nmap

**Date:** june 29, 2026 
**Lab:** Metasploitable2 VM @ 192.168.56.102 
**Command:** `nmap -O 192.168.56.102` 

**Result:** 
Target OS: Linux 2.6.x 
Confirmed by nmap OS fingerprinting.

**Attacker Notes:** 
Linux 2.6.x is an old kernel. Old OS = more known exploits. 
`nmap -O` is loud but gives huge value in recon. 
In a real test I’d slow it down with `-T2` to avoid IDS.
