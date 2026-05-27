CEH Practical Lab — DVWA Webshell Exploitation & SIEM Detection
Overview
This project documents a hands-on cybersecurity lab focused on:
Web application exploitation
Remote command execution (RCE)
Linux post-exploitation enumeration
Apache log analysis
SIEM telemetry investigation
The objective was to simulate a realistic attacker workflow while simultaneously analyzing the generated telemetry from a defender’s perspective.

Lab Architecture
Infrastructure
Windows Server (Active Directory)
Ubuntu Server (Splunk SIEM)
Dedicated DVWA Server
Kali Linux Attacker Machine
Tools & Technologies
DVWA (Damn Vulnerable Web Application)
Kali Linux
Apache2
MariaDB
PHP
Splunk Enterprise
Nmap
Nikto
Gobuster
Burp Suite

Activities Performed
1. Reconnaissance & Enumeration
Performed:
Service discovery
Port scanning
Web fingerprinting
Directory enumeration
Tools used:
Nmap:


Nikto:



2. DVWA Recovery & Troubleshooting
Resolved multiple operational issues including:
Missing DVWA configuration
Apache/PHP integration errors
MariaDB backend installation
Database credential configuration
Database initialization failures
Key skills practiced:
Linux administration
Service troubleshooting
Web application deployment repair

3. Remote Command Execution (RCE)
A controlled PHP webshell was uploaded through the DVWA File Upload vulnerability.
Example payload:
<?php system($_GET['cmd']); ?>


Successfully achieved:
Remote command execution
Linux command interaction
Web server context execution (www-data)

Performed controlled enumeration:
System identification
Network interface discovery
Process inspection
Listening service enumeration

4. Blue Team & SIEM Investigation
Attack telemetry was monitored through:
Apache access logs

Investigated indicators including:
Suspicious GET parameters
cmd= patterns
Webshell activity
Command execution traces
This exercise demonstrated:
Threat hunting concepts
Webshell detection techniques
Offensive-to-defensive workflow correlation

Skills Developed
Offensive Security
Web exploitation
File upload abuse
Remote command execution
Enumeration methodology
Defensive Security
Log analysis
Threat hunting
SIEM investigation
Detection engineering fundamentals
Infrastructure & Operations
Apache troubleshooting
MariaDB administration
Linux server operations
Secure lab segmentation

Key Takeaways
This lab highlighted the importance of:
Proper file upload validation
Least privilege execution
Web application hardening
Continuous monitoring & detection
It also reinforced how offensive activity appears from the defender’s perspective through centralized logging and SIEM analysis.

Disclaimer
This project was conducted entirely inside an isolated private lab environment for educational and authorized security research purposes only.


