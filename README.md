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

- High Severity – SMB Signing Not Required
- Medium Severity – TLS 1.0 Supported (Deprecated)
- Low Severity – Outdated software versions detected (non-critical)

Mitigation strategies were noted for each high/medium vulnerability.

## Output Files

- nessus_scan_report.pdf – Full exported vulnerability report  
- Screenshots(Task-3)/ – Folder with scan setup and results screenshots  

## Outcome  
Gained hands-on experience using Nessus for real-world vulnerability scanning. Understood the scanning process, reading reports, and basic mitigation practices for system security.
