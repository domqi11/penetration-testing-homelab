# Penetration Testing Home Lab: WordPress Vulnerability Assessment

[![Security](https://img.shields.io/badge/Security-Penetration%20Testing-red)](https://github.com/domqi11/pentest-homelab)
[![Platform](https://img.shields.io/badge/Platform-Kali%20Linux-blue)](https://www.kali.org/)
[![Tools](https://img.shields.io/badge/Tools-Metasploit%20%7C%20Nmap%20%7C%20John-orange)](https://www.metasploit.com/)

## 🎯 Project Overview

This repository documents a comprehensive penetration testing assessment conducted in a controlled home lab environment. The project demonstrates end-to-end exploitation of a vulnerable WordPress installation, showcasing real-world attack techniques and methodologies used in cybersecurity assessments.

**⚠️ Educational Purpose Only**: This project is conducted in a controlled lab environment for educational and skill development purposes. All vulnerabilities are exploited on intentionally vulnerable systems with explicit permission.

## 🏗️ Lab Environment

- **Attacker Machine**: Kali Linux (Latest version)
- **Target Machine**: [Basic Pentesting: 1](https://www.vulnhub.com/entry/basic-pentesting-1,216/) from VulnHub
- **Network**: Isolated virtual network (Host-Only/NAT)
- **Virtualization**: VirtualBox/VMware
- **Scope**: Complete authorized penetration test on intentionally vulnerable system

## 🔍 Vulnerabilities Discovered

| # | Vulnerability | Severity | CVSS Score | Impact |
|---|---------------|----------|------------|---------|
| 1 | Default Credentials | **Critical** | 9.0 | WordPress admin access |
| 2 | Remote Code Execution + Privilege Escalation | **Critical** | 9.8 | Complete system compromise |
| 3 | Directory Indexing | **Medium** | 5.3 | Information disclosure |

## 📋 Exploitation Methodology

### Phase 1: Reconnaissance & Discovery
- Network scanning with `nmap`
- Service enumeration
- Directory discovery with `dirb`

### Phase 2: Vulnerability Assessment
- WordPress installation analysis
- Default credential testing
- Security configuration review

### Phase 3: Exploitation
- WordPress admin access via default credentials
- Remote code execution using Metasploit
- System shell acquisition
- Password hash extraction and cracking

### Phase 4: Post-Exploitation
- Privilege escalation to user account
- System persistence demonstration
- Impact assessment

## 🛠️ Tools & Technologies

- **Kali Linux**: Primary penetration testing platform
- **Nmap**: Network discovery and port scanning
- **Dirb**: Directory and file enumeration
- **Metasploit Framework**: Exploitation framework
- **John the Ripper**: Password hash cracking
- **Burp Suite**: Web application security testing
- **Nikto**: Web vulnerability scanner

## 📁 Repository Structure

```
├── README.md                    # This file
├── reports/
│   ├── penetration-test-report.pdf    # Complete assessment report
│   └── vulnerability-summary.md       # Quick reference guide
├── scripts/
│   ├── exploitation-script.md         # Step-by-step exploitation guide
│   └── reconnaissance.sh              # Automated recon script
├── evidence/
│   ├── screenshots/                   # All exploitation evidence
│   └── network-diagrams/              # Lab topology
├── videos/
│   └── demo-links.md                  # Links to demonstration videos
└── remediation/
    └── security-recommendations.md    # Mitigation strategies
```

## 🎥 Video Demonstrations

This project includes comprehensive video demonstrations of each exploitation phase:

1. **Network Discovery & Reconnaissance** (0:00-2:00)
2. **Default Credential Exploitation** (2:00-4:00)
3. **Remote Code Execution & Privilege Escalation** (4:00-8:00)
4. **Directory Indexing Vulnerability** (8:00-9:00)
5. **Impact Assessment & Summary** (9:00-10:00)

*Video links will be added once uploaded to YouTube*

## 🔧 Quick Start Guide

### Prerequisites
- Kali Linux VM or installation
- [Basic Pentesting: 1](https://www.vulnhub.com/entry/basic-pentesting-1,216/) vulnerable VM from VulnHub
- VirtualBox/VMware for virtualization
- Basic knowledge of Linux command line
- Minimum 8GB RAM for smooth VM operation



## 📖 References & Further Reading

- [OWASP Top 10 Web Application Security Risks](https://owasp.org/www-project-top-ten/)
- [NIST Cybersecurity Framework](https://www.nist.gov/cyberframework)
- [Penetration Testing Execution Standard (PTES)](http://www.pentest-standard.org/)
- [Common Vulnerability Scoring System (CVSS)](https://www.first.org/cvss/)

## ⚖️ Legal & Ethical Considerations

- All testing conducted on owned/authorized systems only
- No unauthorized access to third-party systems
- Follows responsible disclosure principles
- Complies with applicable cybersecurity laws and regulations


**⭐ If you found this project helpful, please consider giving it a star!**

*Last updated: June 2025*
