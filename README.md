<h1 align="center">🛡️ Web and Network Pentesting Portfolio</h1>

<p align="center">
  <img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&size=22&duration=3000&pause=1000&color=FF3D3D&center=true&vCenter=true&width=600&lines=Kali+Linux+%7C+Burp+Suite+%7C+Metasploit" alt="Typing SVG" />
</p>

<p align="center"><b>🔓 Cybersecurity Training @ Nitte | Red Team & Forensics | July 2025</b></p>

---

## 📌 About This Repo

This repository documents the hands-on tasks I performed during my **Cybersecurity Internship (July 2025)**, focused on:
- Web application exploitation
- Network attack simulation
- Real-world tool usage and reporting
- Red Team & Forensics skill-building

>  All testing was done in secure labs (custom-hosted vulnerable apps) under ethical conditions.

---

## Tools Used

| Category         | Tools & Frameworks                             |
|------------------|-------------------------------------------------|
| Web Pentesting   | Burp Suite, sqlmap, OWASP ZAP, FFUF, Gobuster   |
| Network Exploits | Nmap, Wireshark, Metasploit, Medusa, Hydra     |
| Forensics        | Autopsy, Volatility, ExifTool                  |
| OS & Platforms   | Kali Linux, Metasploitable2                    |
| Automation       | Bash Scripting, Python                         |

---

##  Vulnerabilities Exploited

> These were identified and exploited in real-world style environments:

- 🔴 **SQL Injection (SQLi)**  
- 🟠 **Cross-Site Scripting (XSS)** – Stored, Reflected, DOM  
- 🔴 **Local File Inclusion (LFI)**  
- 🟡 **Server-Side Template Injection (SSTI)**  
- 🟠 **Insecure Direct Object Reference (IDOR)**  
- 🔴 **Unrestricted File Upload**  
- 🟢 **Privilege Escalation (Windows & Linux)**  
- 🟠 **Network Attacks (FTP anonymous login, SSH brute-force, SMB enumeration)**

---

## 🧠 Real-World Scenarios Documented

-  Attacked custom-hosted vulnerable web apps on Kali using **Burp Suite**, **sqlmap**, and **manual payloads**
-  Discovered misconfigured file upload and directory traversal vulnerabilities
-  Gained unauthorized access via **SMB**, **FTP**, and **brute-force attacks**
-  Captured reverse shells via Metasploit (e.g., MS17-010)
-  Documented all attacks with CVSS scores and mitigations
-  Explored **Microsoft 365** cloud security and **EDR bypasses** in lab
-  Created forensic reports using tools like **Autopsy** and **Volatility** on memory dumps, exfiltrated drives, and steganography challenges

---

## 📁 Walkthrough Index

Each write-up includes: **Setup ➜ Exploit Steps ➜ Screenshot Proof ➜ Mitigation**  
Click to explore:

| Vulnerability / Topic        | Walkthrough Link                                     |
|------------------------------|------------------------------------------------------|
| SQL Injection (sqlmap)       | [`walkthroughs/SQLi-sqlmap.md`](walkthroughs/SQLi.md)     |
| Cross-Site Scripting (XSS)   | [`walkthroughs/XSS-JuiceShop.md`](walkthroughs/XSS.md) |
| Local File Inclusion (LFI)   | [`walkthroughs/LFI-DVWA.md`](walkthroughs/LFI.md)           |
| SMB Enumeration              | [`walkthroughs/SMB-Enum.md`](walkthroughs/SMB-Enum.md)           |
| SSH Brute Force (Medusa)     | [`walkthroughs/SSH-Bruteforce.md`](walkthroughs/SSH.md) |
| SSTI on Flask Apps           | [`walkthroughs/SSTI.md`](walkthroughs/SSTI.md)                   |
| IDOR Access Exploit          | [`walkthroughs/IDOR-Nitte.md`](walkthroughs/IDOR.md)       |

---

## 🧾 Clone This Repo

```bash
git clone https://github.com/shravya235/Penetration-Testing-Portfolio.git
