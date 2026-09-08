# [Domain-1](#domain-1-general-security-concepts) **General Security Concepts**

> 🤖 [AI Tutor](https://edureify.com/certification/exam/comptia-security-plus) · 🎓 [Training](https://edureify.com/certification/cybersecurity/comptia-security-plus/training) · 📝 [Practice Test](https://edureify.com/certification/cybersecurity/comptia-security-plus/practice-test) · 🎯 [Mock Exam](https://edureify.com/certification/cybersecurity/comptia-security-plus/mock-exam) · 📊 [Readiness Test](https://edureify.com/certification/cybersecurity/comptia-security-plus/readiness-test) · 📄 [Cheat Sheet](https://edureify.com/certification/cybersecurity/comptia-security-plus/cheat-sheet) · 📖 [Study Guide](https://edureify.com/certification/cybersecurity/comptia-security-plus/study-guide)

- The smallest domain by weight (**12%**), but its vocabulary is the foundation every other domain builds on — expect terms from here to resurface inside Architecture and Operations questions

## 1.1 Compare and contrast various types of security controls

- Controls are classified along two independent axes — **category** and **type** — and questions often hand you a control and ask you to identify both:
  - **Categories**: Technical (implemented via technology, e.g., firewalls), Managerial (administrative/policy-driven, e.g., a risk assessment process), Operational (implemented by people day-to-day, e.g., security guards, awareness training), Physical (tangible barriers, e.g., locks, fencing)
  - **Types**: Preventive (stops an incident before it happens), Deterrent (discourages an attempt without necessarily stopping it), Detective (identifies an incident in progress or after the fact), Corrective (limits/reverses damage after an incident), Compensating (an alternative when the primary control isn't feasible), Directive (mandates a behavior, e.g., a policy requiring specific action)
- A single control can be described by both axes simultaneously — e.g., a fence is a Physical/Deterrent control; an IDS is a Technical/Detective control

## 1.2 Summarize fundamental security concepts

- **CIA Triad**: Confidentiality, Integrity, Availability — the classic core objectives of security, often extended with **non-repudiation** (a party can't deny an action) and authentication
- **AAA**: Authentication, Authorization, Accounting — identify, decide what's permitted, and log what happened
- **Gap analysis**: comparing current security posture to a desired baseline/framework to identify where controls are missing
- **Zero Trust Architecture**: the modern centerpiece of this objective — "never trust, always verify," with no implicit trust based on network location
  - **Control plane**: includes the **policy engine** (evaluates access requests against policy) and **policy administrator** (executes the policy engine's decision by establishing/terminating the connection)
  - **Data plane**: where the actual traffic subject to the policy decision flows, enforced by policy enforcement points
- **Physical security** fundamentals: fencing, lighting, access control vestibules, and surveillance work together as layered deterrents/detective controls

## 1.3 Explain the importance of change management processes and the impact to security

- **Business process side**: change requests should go through defined approval workflows, with clear ownership and identified stakeholders before implementation — skipping approval is a classic root cause in "what went wrong" scenario questions
- **Technical implications**: allow lists/deny lists, restart/downtime requirements, dependencies between systems, and legacy application compatibility all need to be assessed *before* a change goes live, not discovered after
- **Documentation**: updated diagrams, policies, and procedures should reflect the change once complete — undocumented drift between "what's documented" and "what's actually deployed" is itself a security risk (makes incident response and audits harder)

## 1.4 Explain the importance of using appropriate cryptographic solutions

- The domain's densest objective — a lot of vocabulary that reappears across Architecture (Domain 3) and Operations (Domain 4):
  - **PKI (Public Key Infrastructure)**: certificate authorities, registration authorities, and the trust chain binding public keys to identities
  - **Encryption levels**: full-disk, partition, file, volume, and record-level encryption — each trades off granularity vs. performance/complexity
  - **Symmetric vs. asymmetric encryption**: shared-secret speed vs. public/private-key key-distribution convenience (see also CISSP Domain 3 if cross-studying)
  - **Key exchange**: securely establishing a shared symmetric key over an insecure channel (e.g., Diffie-Hellman)
  - **Digital signatures and certificates**: provide integrity and non-repudiation by combining hashing with asymmetric encryption
  - **Hashing and salting**: hashing creates a fixed-size fingerprint of data (used for integrity verification and password storage); salting adds random data before hashing to defeat precomputed rainbow-table attacks
  - **Blockchain**: a distributed, append-only ledger secured via cryptographic linking of blocks — recognized here as an emerging cryptographic application, not a deep-dive topic
- Know *when* each tool is the right fit (e.g., hashing for integrity/password storage, encryption for confidentiality, signatures for non-repudiation) more than the underlying math
