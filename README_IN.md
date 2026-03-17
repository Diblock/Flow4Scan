



# Flow4Scan – Advanced Nmap Automation & Analysis Tool

> Complete automated scanning, parsing, and analysis pipeline for cybersecurity.
> Reconnaissance → Scanning → Parsing → Analysis → Reporting

---

## 📌 Description

**Flow4Scan** is an advanced tool that automates the entire network auditing workflow. 

It transforms Nmap results into **actionable intelligence**, detecting risks, critical services, and potential attack vectors without requiring manual parsing.

---

## ✨ Main Features

### ⚙️ Complete Automation
* Execution of pre-configured Nmap scans.
* Automatic generation of structured results.
* Security analysis without manual intervention.

### 🔍 Scan Types
* **Fast Scan:** Quick discovery.
* **Aggressive Scan:** Full detection and enumeration.
* **Auto Port Scan:** Smart discovery (fast port scan followed by targeted service scan).
* **Multi Target Scan:** Batch scanning from a file.
* **Full Pro Scan:** Comprehensive scan that includes automated analysis and report generation.
* **UDP Scan:** Requires root privileges.
* **Evasion Scan:** Basic firewall evasion techniques.

---

### 📊 Structured Output

The tool automatically generates the following files after a complete scan:

| File | Description |
| :--- | :--- |
| `scan.xml` | Full raw Nmap XML result |
| `services.json` | Parsed list of detected services |
| `services.csv` | CSV export of open ports and services |
| `summary.json` | High-level numerical summary |
| `analysis.json` | Detailed security analysis and findings |
| `report.md` | Professional Markdown report |
| `report.txt` | Simplified plain-text report |

---

### 🧠 Automated Analysis

Flow4Scan analyzes the data to detect:
* Critical services exposed.
* Risk level classification (LOW / MEDIUM / HIGH / CRITICAL).
* Potential CVEs (based on version heuristics).
* Common attack vectors.
* Insecure default configurations.

---

### 📁 Automatic Organization

Each scan generates its own neatly organized directory with a timestamp:

/output/
└── FullProScan_192.168.1.1_20260316_183000/
    ├── analysis.json
    ├── report.md
    ├── report.txt
    ├── scan.nmap
    ├── scan.xml
    └── services.json

Installation
Clone the repository to your local machine:

https://github.com/Diblock/Flow4Scan.git

Permissions
Give the script execution permissions. Note that some advanced features (like OS detection, SYN stealth scans, and UDP scans) require root privileges:

chmod +x Flow4Scan.sh
sudo ./Flow4Scan.sh

🎯 Use Cases
Basic pentesting and enumeration.

Internal network audits.

Automated network reconnaissance.

Cybersecurity labs and CTFs.

Nmap workflow automation.

⚠️ Limitations
CVE detection is heuristic-based (relies on version matching, not active exploitation).

XML parsing capabilities can be further improved for complex edge cases.

This tool does not replace a thorough manual security audit.

🛡️ Disclaimer
Exclusive use for:

Authorized security audits.

Educational environments.

The author is not responsible for any misuse or damage caused by this tool. Always ensure you have explicit permission to scan a target.

👨‍💻 Author
Francisco Javier Jiménez Cortés

Cybersecurity

Software Development

DevSecOps
