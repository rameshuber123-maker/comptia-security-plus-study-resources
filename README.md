# CompTIA Security+ (SY0-701) Study Resources

Material and resources for pursuing CompTIA Security+ certification — built from the current SY0-701 blueprint, current as of September 2026.

## A note on currency

**SY0-701 is the only active Security+ exam** as of this writing. Its predecessor, SY0-601, retired July 31, 2024. Training-provider chatter points to a possible **SY0-801** successor previewing as early as October 2026, but CompTIA had not confirmed a replacement as of mid-2026 — if you're studying now, sit SY0-701; certifications are valid for 3 years regardless of what launches after, and version transitions historically run long overlap windows.

If a study resource you're using describes six domains, or a domain called "Technologies and Tools" or "Attacks/Threats/Vulnerabilities," it's describing a retired version (SY0-501 or SY0-601) — discard it.

## Table of contents

- [Overview](#overview)
- [Practice with Edureify](#-practice-with-edureify)
- [Reference Material](#reference-material)
- [Study Guides By Domain](#study-guides-by-domain)

## Overview

- **Who is it for?** Security+ is CompTIA's foundational, vendor-neutral security certification — aimed at early-career security/IT professionals rather than deep specialists. No formal prerequisites, though CompTIA recommends prior Network+ knowledge or equivalent experience.
- **Exam format:**
  - Up to 90 questions, 90 minutes, multiple-choice + performance-based questions (PBQs — simulated tasks like ordering firewall rules or reading logs)
  - Passing score: 750 on a 100–900 scale
  - Renewal: every 3 years via CompTIA's Continuing Education (CE) program
- **Domain weights (objectives document v5.0):**

| Domain | Weight |
|---|---|
| 1. General Security Concepts | 12% |
| 2. Threats, Vulnerabilities, and Mitigations | 22% |
| 3. Security Architecture | 18% |
| 4. Security Operations | 28% |
| 5. Security Program Management and Oversight | 20% |

- **Study order that follows the weights**: Security Operations (28%, the heaviest and most scenario/PBQ-dense domain) → Threats/Vulnerabilities/Mitigations (22%) → Security Program Management and Oversight (20%, GRC-heavy — don't leave it to the last minute if you're from a technical background) → Security Architecture (18%) → General Security Concepts (12%, foundational vocabulary that still shows up inside every other domain's questions)
- **Test-taking strategies**
  - PBQs cluster heavily in the "Given a scenario…" objectives, concentrated in Domain 4 — practice log-reading, rule-ordering, and topology placement specifically, not just multiple choice
  - Security+ rewards recognizing *categories* (which control type, which threat actor, which attack technique) as much as memorizing specific product names
  - Build a small home lab (VirtualBox/VMware) to make hardening, logging, and network segmentation concepts concrete rather than abstract

## 🎯 Practice with Edureify

- 🤖 [AI Tutor](https://edureify.com/certification/exam/comptia-security-plus)
- 🎓 [Training](https://edureify.com/certification/cybersecurity/comptia-security-plus/training)
- 📝 [Practice Test](https://edureify.com/certification/cybersecurity/comptia-security-plus/practice-test)
- 🎯 [Mock Exam](https://edureify.com/certification/cybersecurity/comptia-security-plus/mock-exam)
- 📊 [Readiness Test](https://edureify.com/certification/cybersecurity/comptia-security-plus/readiness-test)
- 📄 [Cheat Sheet](https://edureify.com/certification/cybersecurity/comptia-security-plus/cheat-sheet)
- 📖 [Study Guide](https://edureify.com/certification/cybersecurity/comptia-security-plus/study-guide)
- 🏠 [Exam Landing Page](https://edureify.com/certification/cybersecurity/comptia-security-plus/landing)

## Reference Material

- [Official CompTIA Security+ page](https://www.comptia.org/en-us/certifications/security/) — download the current objectives PDF here; always the primary source
- [NIST Cybersecurity Framework (CSF) 2.0](https://www.nist.gov/cyberframework)
- [MITRE ATT&CK](https://attack.mitre.org/) — useful for Domain 2/4 threat and detection concepts
- [OWASP Top 10](https://owasp.org/www-project-top-ten/) — relevant to Domain 2's web/application vulnerabilities

## Study Guides By Domain

- [Domain 1 - General Security Concepts (12%)](Security-Plus-Domain-1-Objectives.md)
- [Domain 2 - Threats, Vulnerabilities, and Mitigations (22%)](Security-Plus-Domain-2-Objectives.md)
- [Domain 3 - Security Architecture (18%)](Security-Plus-Domain-3-Objectives.md)
- [Domain 4 - Security Operations (28%)](Security-Plus-Domain-4-Objectives.md)
- [Domain 5 - Security Program Management and Oversight (20%)](Security-Plus-Domain-5-Objectives.md)
