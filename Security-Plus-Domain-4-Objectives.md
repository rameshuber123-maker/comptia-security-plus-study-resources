# [Domain-4](#domain-4-security-operations) **Security Operations**

> 🤖 [AI Tutor](https://edureify.com/certification/exam/comptia-security-plus) · 🎓 [Training](https://edureify.com/certification/cybersecurity/comptia-security-plus/training) · 📝 [Practice Test](https://edureify.com/certification/cybersecurity/comptia-security-plus/practice-test) · 🎯 [Mock Exam](https://edureify.com/certification/cybersecurity/comptia-security-plus/mock-exam) · 📊 [Readiness Test](https://edureify.com/certification/cybersecurity/comptia-security-plus/readiness-test) · 📄 [Cheat Sheet](https://edureify.com/certification/cybersecurity/comptia-security-plus/cheat-sheet) · 📖 [Study Guide](https://edureify.com/certification/cybersecurity/comptia-security-plus/study-guide)

- The exam's heavyweight domain at **28%** — nine sub-objectives, and the highest concentration of "Given a scenario…" performance-based questions in the whole exam. If your study time is rationed anywhere, don't ration it here.

## 4.1 Given a scenario, apply common security techniques to computing resources

- **Secure baselines**: establish, deploy, and maintain a hardened standard configuration — the reference point every deployed system should match
- **Hardening targets**: spans mobile devices, servers, workstations, and even ICS — hardening steps (disabling unused services, closing ports, removing default credentials) apply everywhere but details differ by platform
- **Wireless security**: WPA3 (current standard), RADIUS (centralized authentication), and site surveys (mapping real-world signal coverage/interference before deployment)
- **Mobile solutions**: MDM (Mobile Device Management), and deployment models — BYOD (Bring Your Own Device), COPE (Corporate-Owned, Personally Enabled), CYOD (Choose Your Own Device) — each shifts the ownership/control balance differently
- **Application security and sandboxing**: isolating untrusted code/applications in a contained environment to limit potential damage

## 4.2 Explain the security implications of proper hardware, software, and data asset management

- **Acquisition**: security requirements should be built into procurement, not added afterward
- **Assignment and accounting**: clear ownership, classification, and inventory tracking throughout an asset's life (echoes CISSP Domain 2 concepts)
- **Disposal**: sanitization and destruction appropriate to data sensitivity, with certification of destruction where required, and awareness of data-retention obligations that might require keeping (not destroying) certain records

## 4.3 Explain various activities associated with vulnerability management

- **Identification methods**: vulnerability scans, application security analysis, threat intelligence feeds, penetration testing, and bug bounty programs
- **Analysis**: CVSS (Common Vulnerability Scoring System — severity scoring) and CVE (Common Vulnerabilities and Exposures — the standard identifier for a known vulnerability), plus distinguishing true findings from false positives, and prioritizing by actual business risk, not raw score alone
- **Response**: patching, cybersecurity insurance, segmentation, and compensating controls when a direct fix isn't immediately possible
- **Validation**: confirming remediation worked via rescanning, audit, and reporting — a vulnerability isn't closed until verified, not just "patched and assumed fixed"

## 4.4 Explain security alerting and monitoring concepts and tools

- Covers both **monitoring computing resources** and **alert response/remediation** workflows
- Core tool stack to know by purpose (tool-to-purpose matching is a common question format):
  - **SIEM (Security Information and Event Management)**: centralizes and correlates log data for detection
  - **SCAP (Security Content Automation Protocol)**: standardizes vulnerability/configuration compliance checking
  - **Antivirus, DLP (Data Loss Prevention), SNMP traps, NetFlow, vulnerability scanners**: each addresses a distinct layer — endpoint malware, data exfiltration, device health alerts, network traffic pattern analysis, and known-weakness detection respectively

## 4.5 Given a scenario, modify enterprise capabilities to enhance security

- **Firewall rules and screened subnets (DMZs)**: rule ordering matters — more specific rules typically must precede general ones, a classic PBQ exercise
- **IDS/IPS signatures**: keeping detection signatures current is as important as having the tool deployed
- **Web and DNS filtering**: blocking access to malicious or policy-violating destinations before a connection completes
- **OS security**: Group Policy (Windows) and SELinux (Linux) enforce security configuration at the operating-system level
- **Secure protocol selection**: choosing encrypted/authenticated protocol variants (e.g., HTTPS over HTTP, SFTP over FTP) wherever a legacy insecure option exists
- **Email security**: DMARC, DKIM, and SPF work together to prevent email spoofing and verify sender legitimacy
- **File integrity monitoring, NAC, and EDR/XDR**: detect unauthorized file changes, enforce device compliance before network access, and provide endpoint (and cross-domain, for XDR) detection/response respectively

## 4.6 Given a scenario, implement and maintain identity and access management

- **Provisioning and deprovisioning**: timely access lifecycle management (see CISM/CISSP IAM domains for the same underlying principle)
- **Federation and SSO**: SAML and OAuth as the standard protocols enabling single sign-on across systems
- **MFA**: factors and implementation methods — something you know/have/are, combined for stronger authentication
- **Password best practices and password managers**: complexity/length guidance has shifted toward length and uniqueness (via managers) over frequent forced rotation
- **Privileged Access Management (PAM)**: additional controls (vaulting, session recording, just-in-time elevation) specifically for high-privilege accounts

## 4.7 Explain the importance of automation and orchestration related to secure operations

- **Use cases**: automated user provisioning, ticket creation, enforcing configuration "guardrails," and security-group management at scale
- **Benefits**: efficiency, consistently enforced baselines, and faster reaction time than manual processes allow
- **Honest costs**: added complexity, potential technical debt, and the risk that automation itself becomes a single point of failure if misconfigured — automation should be evaluated on both benefit and risk, not assumed to be a free win

## 4.8 Explain appropriate incident response activities

- **Lifecycle**: Preparation → Detection → Analysis → Containment → Eradication → Recovery → Lessons Learned (closely mirrors the NIST SP 800-61 lifecycle referenced in other security certifications)
- **Supporting activities**: incident response training, tabletop exercises, root cause analysis, and proactive threat hunting
- **Digital forensics fundamentals**: legal hold (preserving evidence once litigation/investigation is reasonably anticipated), chain of custody, and proper evidence acquisition/preservation — mishandling any of these can make evidence unusable

## 4.9 Given a scenario, use data sources to support an investigation

- **Log data sources**: firewall, application, endpoint, OS-specific, IPS/IDS, network, and metadata logs — each answers different investigative questions
- **Other sources**: vulnerability scan results, automated reports, dashboards, and packet captures
- Expect scenario-style questions that hand you excerpts from one or more of these sources and ask what occurred — practicing actual log reading is more valuable here than memorizing definitions
