# [Domain-2](#domain-2-threats-vulnerabilities-and-mitigations) **Threats, Vulnerabilities, and Mitigations**

> 🤖 [AI Tutor](https://edureify.com/certification/exam/comptia-security-plus) · 🎓 [Training](https://edureify.com/certification/cybersecurity/comptia-security-plus/training) · 📝 [Practice Test](https://edureify.com/certification/cybersecurity/comptia-security-plus/practice-test) · 🎯 [Mock Exam](https://edureify.com/certification/cybersecurity/comptia-security-plus/mock-exam) · 📊 [Readiness Test](https://edureify.com/certification/cybersecurity/comptia-security-plus/readiness-test) · 📄 [Cheat Sheet](https://edureify.com/certification/cybersecurity/comptia-security-plus/cheat-sheet) · 📖 [Study Guide](https://edureify.com/certification/cybersecurity/comptia-security-plus/study-guide)

- The exam's second-heaviest domain at **22%** — largely a "know your enemy" recognition domain: identify the actor, the vector, the vulnerability, or the indicator from a description

## 2.1 Compare and contrast common threat actors and motivations

- **Actor types**: nation-state (highest resources/sophistication, espionage/disruption motives), organized crime (financially motivated), hacktivists (ideologically motivated), insiders (existing legitimate access — often the hardest to detect), unskilled/script-kiddie attackers (low sophistication, often opportunistic), and shadow IT (not malicious, but unmanaged/ungoverned technology use that creates risk)
- Compare actors along consistent axes: **internal vs. external**, **level of resources/funding**, and **level of sophistication/capability** — these axes are how exam questions typically differentiate similar-sounding options

## 2.2 Explain common threat vectors and attack surfaces

- **Vectors** describe *how* an attack reaches its target: message-based (email, SMS), image-based (malicious payloads hidden in image files), file-based, voice (vishing calls), removable media (USB drops), unsecured/open networks and ports, and supply chain (compromising a trusted vendor/component to reach the real target)
- **Human-vector/social engineering catalog**: phishing (broad email-based), smishing (SMS), vishing (voice), pretexting (fabricated scenario to extract information), business email compromise (impersonating a trusted executive/vendor to redirect payments), and watering-hole attacks (compromising a site the target is known to visit)

## 2.3 Explain various types of vulnerabilities

- **Application**: memory injection, buffer overflow, race conditions — flaws in how software is written
- **Operating system**: unpatched or misconfigured OS-level weaknesses
- **Web**: SQL injection (SQLi) and cross-site scripting (XSS) are the two headline examples — both stem from insufficient input validation
- **Hardware**: firmware vulnerabilities and end-of-life devices that no longer receive security updates
- **Virtualization**: VM escape — a guest VM breaking out to affect the host or other VMs
- **Cloud-specific**: misconfigured storage/permissions, insecure APIs, and shared-tenancy risks
- **Supply chain, misconfiguration, mobile, and zero-day vulnerabilities** round out the category — a zero-day is a vulnerability unknown to the vendor (no patch yet available), making it especially dangerous

## 2.4 Given a scenario, analyze indicators of malicious activity

- This objective is the domain's scenario workhorse — you're handed symptoms/log evidence and asked to identify the attack
- **Malware types**: ransomware (encrypts data for extortion), trojan (disguised as legitimate software), worm (self-propagating without user action), spyware (covertly collects information), rootkit (hides its presence, often at a privileged/kernel level)
- **Physical and network attacks**: DDoS (overwhelming a target with traffic from many sources), DNS attacks (e.g., poisoning), on-path/man-in-the-middle attacks, and credential replay (reusing captured authentication material)
- **Application attacks**: injection attacks, privilege escalation (gaining higher access than intended), and directory traversal (accessing files outside an intended directory)
- **Cryptographic attacks**: recognizing described evidence of brute-force, downgrade, or collision-style attacks from a scenario

## 2.5 Explain the purpose of mitigation techniques used to secure the enterprise

- This objective pairs directly with 2.4: given the attack identified above, choose the appropriate mitigation
- Core techniques: **segmentation** (limiting lateral movement), **access control** (least privilege), **isolation** (quarantining affected systems), **patching** (closing known vulnerabilities), **encryption** (protecting confidentiality even if data is accessed), **monitoring** (detecting ongoing/repeat attempts), **configuration enforcement** (preventing drift from a secure baseline), **decommissioning** (removing unused/unsupported systems that expand attack surface), and **hardening** (reducing a system's attack surface generally — disabling unneeded services, closing unused ports)
