# Nmap Network Reconnaissance & Port Scanning Lab

## Overview
This project demonstrates how a Security Operations Center (SOC) analyst can use Nmap
to perform network reconnaissance, identify exposed services, and assess potential attack surface.

The lab simulates an internal security assessment by scanning localhost and the local subnet
to identify open ports, running services, operating system fingerprints, and potential
security weaknesses. The goal was to replicate the reconnaissance phase of a real-world attack
and document findings in a structured, professional format.

---

## Objectives
- Perform host discovery and port scanning
- Identify exposed services and service versions
- Detect operating system fingerprints
- Execute Nmap Scripting Engine (NSE) scripts
- Analyze potential security risks
- Document findings like a SOC analyst

---

## Skills Demonstrated
- Network reconnaissance
- TCP SYN scanning
- Service version detection
- OS fingerprinting
- NSE script execution
- Attack surface analysis
- Security documentation & reporting

---

## Tools Used
- Nmap
- Windows Command Prompt
- Localhost test environment
- Private local network (192.168.x.0/24)

---

# 🔍 Phase 1 – Basic Host Scan

### Command Used


### Purpose
Performed a TCP SYN (stealth) scan to identify open TCP ports on the local machine.

### Screenshot
![Basic Scan](screenshots/01-basic-scan.png)

### Analyst Insight
This scan identifies exposed services that could be targeted during reconnaissance.
Open ports increase the system’s attack surface.

---

# 🌐 Phase 2 – Local Network Discovery

### Command Used

The `-A` flag enables:
- OS detection
- Version detection
- Script scanning
- Traceroute

---

## Open Ports & Service Versions

![Advanced Scan - Ports](screenshots/03-advanced-scan-ports.png)

### Analysis
This section identifies:
- Open TCP ports
- Running services
- Service version information

Service version detection is critical for vulnerability assessment,
as outdated services may contain known exploits.

---

## Operating System Fingerprinting

![Advanced Scan - OS](screenshots/04-advanced-scan-os.png)

### Analysis
OS detection provides:
- Estimated operating system
- Network distance
- Host fingerprinting data

Attackers use OS detection to tailor exploitation techniques.

---

## Nmap Scripting Engine (NSE) Results

![Advanced Scan - Scripts](screenshots/05-advanced-scan-scripts.png)

### Analysis
NSE scripts provide deeper visibility into:
- Service configurations
- Protocol behavior
- Potential security weaknesses

This stage simulates deeper reconnaissance during the pre-exploitation phase.

---

# 🔐 Security Findings & Risk Assessment

Based on scan results:

- Open ports represent exposed entry points
- Service versions may indicate outdated software
- OS fingerprinting confirms host environment
- Script outputs reveal configuration details

Even when scanning localhost, this demonstrates how attackers
enumerate systems prior to exploitation attempts.

---

# 🛡 SOC Perspective

From a SOC analyst standpoint, this project demonstrates:

- Understanding of reconnaissance techniques
- Ability to interpret scan output
- Identification of attack surface exposure
- Structured documentation of findings
- Awareness of ethical scanning boundaries

Network reconnaissance is typically the first phase of an intrusion.
Proper monitoring, firewall controls, and service hardening are critical
to reducing exposure.

---

# Key Takeaways
- Open ports increase system risk
- Service version detection assists vulnerability management
- OS fingerprinting enhances threat intelligence context
- Reconnaissance tools are powerful and must be monitored
- Documentation is essential for security reporting

---

## Disclaimer
All scans were conducted against localhost and privately owned devices
within a controlled lab environment. No unauthorized systems were scanned.
This project was performed strictly for educational purposes.
