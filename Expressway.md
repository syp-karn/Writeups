![image.png](img/Expressway/image.png)


# Nmap Scan

```bash
nmap -p $(cat ports.txt ) -sVC -O --min-rate=1000 10.129.16.8
Starting Nmap 7.95 ( https://nmap.org ) at 2026-01-19 19:06 IST
Nmap scan report for 10.129.16.8
Host is up (0.058s latency).

PORT   STATE SERVICE VERSION
22/tcp open  ssh     OpenSSH 10.0p2 Debian 8 (protocol 2.0)
Warning: OSScan results may be unreliable because we could not find at least 1 open and 1 closed port
Aggressive OS guesses: Linux 4.15 - 5.19 (98%), Android 9 - 10 (Linux 4.9 - 4.14) (94%), Linux 3.2 - 4.14 (94%), Linux 2.6.32 - 3.10 (93%), MikroTik RouterOS 7.2 - 7.5 (Linux 5.6.3) (93%), OpenWrt 21.02 (Linux 5.4) (93%), Linux 2.6.32 (92%), Linux 6.0 (92%), Linux 4.19 (91%), Linux 2.6.32 - 3.5 (90%)
No exact OS matches for host (test conditions non-ideal).
Service Info: OS: Linux; CPE: cpe:/o:linux:linux_kernel

OS and Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
Nmap done: 1 IP address (1 host up) scanned in 10.50 seconds

```

The Nmap scan shows only an SSH service running on port 22; nothing else.


*This box is still active on HackTheBox. Once retired, this writeup will be published for public access as per HackTheBox's policy on publishing content from their platform*