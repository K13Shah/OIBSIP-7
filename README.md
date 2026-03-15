# Web Vulnerability Scanner (Linux)

A simple automated toolkit for **scanning and analyzing vulnerabilities in a target web server** using Linux security tools.

⚠️ **Disclaimer:**
This tool is intended **only for authorized security testing and educational purposes**. Do not scan systems without proper permission.

---

## Features

* Port and service scanning
* Web server vulnerability detection
* Technology fingerprinting
* Automated result collection
* Basic vulnerability analysis

---

## Tools Used

* Nmap – Network and port scanner
* Nikto – Web server vulnerability scanner
* WhatWeb – Website technology detection
* OWASP ZAP – Web application security scanner
* Python – Result analysis automation

---

## Installation

```bash
sudo apt update
sudo apt install nmap nikto whatweb zaproxy python3 -y
```

---

## Usage

Run the scanner:

```bash
chmod +x web_vuln_scan.sh
./web_vuln_scan.sh <target-domain>
```

Example:

```bash
./web_vuln_scan.sh example.com
```

Analyze results:

```bash
python3 analyze_results.py
```

---

## Output

The scanner creates a directory:

```
scan_results_<target>
```

It contains:

* Nmap scan results
* Nikto vulnerability report
* WhatWeb technology detection
* OWASP ZAP security report

---

## Author

Security Research / Ethical Hacking Project
