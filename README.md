# Task 3: Basic Vulnerability Scan on Your PC

## Objective  
Perform a basic vulnerability scan on my personal system using a free vulnerability scanner to identify common system flaws and weaknesses.

## Tools Used  
- Nessus Essentials – Free edition by Tenable for vulnerability scanning  
- Localhost IP (127.0.0.1) as the scan target  
- Windows 10 OS as the system under test  

## Steps Performed  

1. Installed and activated Nessus Essentials.
2. Added a new scan using Basic Network Scan.
3. Set the scan target as localhost (127.0.0.1).
4. Launched the scan and waited ~30–45 minutes for it to complete.
5. Reviewed the full vulnerability report for:
   - High/critical vulnerabilities
   - CVE references
   - Suggested fixes
6. Exported the final scan report as PDF for documentation.
7. Took relevant screenshots of scan setup, progress, and results.

## Key Findings 

- Multiple High-Risk Vulnerabilities in Node.js  
  - Detected version: 20.11.0  
  - Affected by CVEs like CVE-2024-21892, CVE-2024-22019, and more  
  - Risks: DoS, path traversal, privilege escalation, side-channel attacks  
  - **Fix**: Update Node.js to 20.18.2 or later

- Untrusted SSL Certificate Detected  
  - Self-signed Nessus certificate not issued by a known CA  
  - Fix: Replace with a valid certificate from a trusted authority

- Apache Log4j Presence Detected  
  - Versions 2.17.1 and 2.24.2 found  
  - No active vulnerability detected but still a risk due to past critical issues  
  - Fix: Keep updated and monitor configuration

- Apache HTTP Server Identified  
  - Version 2.4.63  
  - No immediate issues flagged, but continued patching is essential

- Dockerfile and Tool Exposure  
  - Metasploit, ZAP, and Zphisher tools detected  
  - If containers are misconfigured, this could expose services  
  - Fix: Harden containers and restrict public access

- Node.js Permission Model Path Traversal Risks  
  - Misconfigurations allow bypassing of fs-read/write flags  
  - Fix: Avoid enabling experimental features in production
Mitigation strategies were noted for each high/medium vulnerability.

## Output Files

- nessus_scan_report.pdf – Full exported vulnerability report  
- Screenshots(Task-3)/ – Folder with scan setup and results screenshots  

## Outcome  
Gained hands-on experience using Nessus for real-world vulnerability scanning. Understood the scanning process, reading reports, and basic mitigation practices for system security.
