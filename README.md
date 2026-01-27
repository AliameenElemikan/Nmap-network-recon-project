# Nmap Local Lab: Service Discovery + Security Hardening Report

## Overview
This project demonstrates ethical network reconnaissance in a controlled lab environment using Nmap.
The goal is to identify open ports, detect running services, and produce a defensive hardening report
based on the results.

## Objectives
- Discover open ports on a lab-owned target
- Identify services and versions (service enumeration)
- Run safe NSE scripts for basic security insights
- Save outputs in readable and structured formats
- Provide remediation/hardening recommendations

## Tools Used
- Nmap (free)
- (Optional) VirtualBox/VMware for a target VM

## Ethics / Scope
All scans were performed only against systems I own or have explicit permission to test
(e.g., my own machine or a local VM). No scanning of public IPs or unauthorized networks.

## Commands Used
### 1) Basic service + OS detection
```bash
nmap -sV -O <TARGET_IP> -oN scans/basic.txt
