# Ramnit Endpoint Forensics Lab

## Overview
This repo documents my analysis of the CyberDefenders Ramnit blue team lab. The goal was to investigate a memory dump using Volatility 3, identify malicious activity, extract IOCs, and correlate findings with threat intelligence.

> No malware samples or memory dumps are included in this repository.

## Lab Details
- Platform: CyberDefenders
- Category: Endpoint Forensics
- Difficulty: Easy
- Role Practice: SOC Analyst Tier 1
- Tools: Volatility 3, VirusTotal
- Tactics: Execution, Defense Evasion, Command and Control

## Scenario
A suspicious process was discovered in a memory dump. The investigation focused on identifying the malicious executable, network communication, file hash, compilation timestamp, and related domain.

## Tools Used
- Volatility 3
- VirusTotal
- Windows PowerShell
- CyberDefenders lab environment

## Investigation Steps

### 1. Process Investigation
Used Volatility 3 to inspect running processes and identify suspicious activity.

Key finding:

```text
Suspicious Process: ChromeSetup.exe
Path: C:\Users\alex\Downloads\ChromeSetup.exe
