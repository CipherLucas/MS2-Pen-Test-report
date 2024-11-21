# Metasploitable VM Penetration Test Report

This repository documents a penetration test conducted on **Rapid7's Metasploitable 2 VM**, an intentionally vulnerable operating system used for security training and testing. The report details the methodology, tools, findings, and recommendations from the assessment.

## Purpose

The penetration test aimed to:
- Identify vulnerabilities in the Metasploitable 2 environment.
- Exploit these vulnerabilities to demonstrate real-world attack vectors.
- Provide actionable recommendations to improve security.

## Summary

The report includes:
- **Scope of Testing**: Defined target system, tools, and testing environment.
- **Methodology**: Step-by-step approach including reconnaissance, vulnerability analysis, exploitation, and post-exploitation.
- **Findings**: Critical vulnerabilities in services such as FTP and SMB, including specific CVEs.
- **Exploitation Details**: Examples of successful attacks using tools like Nmap and Metasploit.
- **Recommendations**: Steps to mitigate identified vulnerabilities and harden the system.

## Tools and Techniques

The following tools and techniques were used during the assessment:
- **Nmap**: For network discovery and port scanning.
- **Nessus**: For vulnerability assessment.
- **Metasploit Framework**: For exploiting identified vulnerabilities.

## Key Findings

- **Critical Vulnerabilities**:
  - Vsftpd 2.3.4 Backdoor (CVE-2011-2523)
  - SMB Misconfiguration (CVE-2007-2447)
- **Successful Exploitation**:
  - Root access via FTP and SMB exploits.
  - Discovery of hashed passwords (unencrypted).

## Recommendations

- Upgrade or disable vulnerable services like Vsftpd 2.3.4.
- Harden configurations for services such as SMB.
- Regularly perform vulnerability assessments and apply security patches.

## Conclusion

This report highlights the importance of securing configurations and updating systems regularly. By addressing the findings, the security of the Metasploitable 2 environment can be significantly improved.

---

For more details, refer to the full report in this repository.
