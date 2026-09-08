# [Domain-5](#domain-5-security-program-management-and-oversight) **Security Program Management and Oversight**

> 🤖 [AI Tutor](https://edureify.com/certification/exam/comptia-security-plus) · 🎓 [Training](https://edureify.com/certification/cybersecurity/comptia-security-plus/training) · 📝 [Practice Test](https://edureify.com/certification/cybersecurity/comptia-security-plus/practice-test) · 🎯 [Mock Exam](https://edureify.com/certification/cybersecurity/comptia-security-plus/mock-exam) · 📊 [Readiness Test](https://edureify.com/certification/cybersecurity/comptia-security-plus/readiness-test) · 📄 [Cheat Sheet](https://edureify.com/certification/cybersecurity/comptia-security-plus/cheat-sheet) · 📖 [Study Guide](https://edureify.com/certification/cybersecurity/comptia-security-plus/study-guide)

- The GRC (Governance, Risk, Compliance) domain, at a full **20%** of the exam — SY0-701 expanded this substantially compared to its predecessor, and candidates from purely technical backgrounds tend to under-prepare for it

## 5.1 Summarize elements of effective security governance

- **Guidelines** (recommended, flexible) vs. **policies** (mandatory statements of intent — AUP, information security policy, business continuity policy, incident response policy) vs. **standards** (mandatory specifics — password standard, access control standard, encryption standard) vs. **procedures** (mandatory step-by-step instructions — change management, onboarding/offboarding)
- **External considerations**: regulatory, legal, and industry-specific requirements shape governance from outside the organization
- **Monitoring and revision**: governance documentation should be periodically reviewed and updated, not written once and forgotten
- **Governance structures**: boards and committees provide oversight and decision-making authority
- **Roles**: owners, controllers, processors, custodians — the same data-role vocabulary used across other security certifications (see CISSP Domain 2)

## 5.2 Explain elements of the risk management process

- **Risk identification and assessment types**: ad hoc, recurring, one-time, and continuous assessments each suit different situations
- **Analysis**: qualitative (descriptive) vs. quantitative — **SLE (Single Loss Expectancy)**, **ALE (Annualized Loss Expectancy)**, **ARO (Annualized Rate of Occurrence)** — ALE = SLE × ARO
- **Risk register, tolerance, and appetite**: the central tracking artifact, and the organization's willingness to accept risk in general (appetite) vs. for a specific risk (tolerance)
- **Management strategies**: transfer, accept, avoid, mitigate — the same four classic responses used throughout risk-focused certifications
- **Business Impact Analysis (BIA)**: RTO (Recovery Time Objective), RPO (Recovery Point Objective), MTTR (Mean Time To Repair), and MTBF (Mean Time Between Failures) — quantify how much downtime/data loss is tolerable and how reliable a system is expected to be

## 5.3 Explain the processes associated with third-party risk assessment and management

- **Vendor assessment**: due diligence, right-to-audit clauses, and supply-chain analysis before engaging a vendor
- **Selection and agreement types**: SLA (Service Level Agreement), MOU (Memorandum of Understanding), MSA (Master Service Agreement), NDA (Non-Disclosure Agreement), and other contract types — know what each formalizes
- **Vendor monitoring**: ongoing assessment doesn't stop once a contract is signed
- **Questionnaires**: standardized vendor security questionnaires are a common, scalable way to gather assurance across many vendors at once

## 5.4 Summarize elements of effective security compliance

- **Reporting**: internal (to leadership/board) and external (to regulators, customers, or the public where required)
- **Consequences of non-compliance**: fines, sanctions, reputational damage, and contractual impacts — compliance failures have both legal and business consequences
- **Monitoring and attestation**: ongoing verification plus formal statements (attestations) that requirements are being met
- **Privacy obligations**: legal implications, the data-subject/controller/processor relationship (again mirroring GDPR-style vocabulary), and rights like the "right to be forgotten"

## 5.5 Explain types and purposes of audits and assessments

- **Attestation**: a formal statement (often from a qualified third party) that a control or process meets a stated standard
- **Internal audits**: compliance checks, audit committees, and self-assessments performed within the organization
- **External audits**: regulatory examinations and independent third-party assessments — carry more weight due to independence
- **Penetration testing concepts**: offensive vs. defensive framing, and environment knowledge levels — known environment (full information provided), partially known, and unknown (black-box, simulating a real external attacker) — plus reconnaissance as the testing process's first phase

## 5.6 Given a scenario, implement security awareness practices

- **Phishing campaigns and recognition training**: simulated phishing to build and measure staff detection ability
- **Anomalous behavior recognition**: training staff to notice and report unusual activity, not just avoid clicking bad links
- **User guidance and training topics**: policy awareness, situational awareness, insider threat indicators, password management, and social engineering resistance generally
- **Reporting and monitoring**: awareness programs should have a clear reporting channel and track effectiveness over time (e.g., improving phishing-simulation results), not just track completion
