<h1 align="center">🛡️ Web and Network Pentesting Portfolio 🕵️‍♀️</h1>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=22&pause=1000&color=F70D1A&center=true&vCenter=true&width=500&lines=Offensive+Security+in+Action...;Burp+Suite+%7C+Kali+Linux+%7C+Metasploit+%7C+CTF+Walkthroughs" alt="Typing SVG" />
</p>

---

##  About This Repo

This repository is a curated collection of **real-world offensive security tasks** I performed during my **Cybersecurity Internship (July 2025)**. It covers detailed walkthroughs of:
-  Web app pentesting
-  Network exploitation
-  Vulnerability discovery
-  Exploits & post-exploitation

All exercises were tested in safe labs like **DVWA**, **Juice Shop**, **Metasploitable2**, and **TryHackMe** boxes — with proper tooling and ethical scope.

---

##  Tools Used

| Category         | Tools & Frameworks                             |
|------------------|-------------------------------------------------|
| Web Pentesting   | Burp Suite, sqlmap, OWASP ZAP, FFUF, Gobuster   |
| Network Exploits | Nmap, Wireshark, Metasploit, Medusa, Hydra     |
| Forensics        | Autopsy, Volatility, ExifTool                  |
| OS & Platforms   | Kali Linux, Metasploitable2                    |
| Automation       | Bash Scripting, Python                         |

---

## 💣 Vulnerabilities Exploited

> These are not just concepts — I manually exploited these in lab setups and captured screenshots, payloads, and impact reports.

- 🔴 **SQL Injection (SQLi)**  
- 🟠 **Cross-Site Scripting (XSS)** – Reflected, Stored, DOM  
- 🔴 **Local File Inclusion (LFI)**  
- 🟡 **Server-Side Template Injection (SSTI)**  
- 🟠 **Broken Access Control (IDOR)** – Horizontal & Vertical  
- 🔴 **File Upload Bypass**  
- 🟢 **Privilege Escalation (Linux/Windows)**  
- 🟠 **Network Exploits (Anonymous FTP, SSH Brute Force)**

---

##  Walkthrough Index

Each write-up includes: **Setup ➜ Exploit Steps ➜ Screenshot Proof ➜ Mitigation**  
Click to explore:

| Vulnerability            | Walkthrough Link                                     |
|--------------------------|------------------------------------------------------|
| SQLi using sqlmap      | [`walkthroughs/SQLi-sqlmap.md`](walkthroughs/SQLi-sqlmap.md)     |
| XSS on Juice Shop      | [`walkthroughs/XSS-JuiceShop.md`](walkthroughs/XSS-JuiceShop.md) |
| LFI on DVWA            | [`walkthroughs/LFI-DVWA.md`](walkthroughs/LFI-DVWA.md)           |
| SMB Enumeration        | [`walkthroughs/SMB-Enum.md`](walkthroughs/SMB-Enum.md)           |
| SSH Brute Force (Medusa)| [`walkthroughs/SSH-Bruteforce.md`](walkthroughs/SSH-Bruteforce.md) |
| Metasploit Exploits    | [`walkthroughs/MS17_010.md`](walkthroughs/MS17_010.md)           |
| IDOR Access Bypass     | [`walkthroughs/IDOR-Nitte.md`](walkthroughs/IDOR-Nitte.md)       |
| SSTI in Flask Apps     | [`walkthroughs/SSTI.md`](walkthroughs/SSTI.md)                   |

> ⚠️ All vulnerable apps were deployed in isolated VMs and containers. Do **not** attempt these techniques on any production or unauthorized systems.

---

```bash
git clone https://github.com/shravya/Web-Network-Pentesting-Portfolio.git
