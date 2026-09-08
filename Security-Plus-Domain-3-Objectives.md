# [Domain-3](#domain-3-security-architecture) **Security Architecture**

> 🤖 [AI Tutor](https://edureify.com/certification/exam/comptia-security-plus) · 🎓 [Training](https://edureify.com/certification/cybersecurity/comptia-security-plus/training) · 📝 [Practice Test](https://edureify.com/certification/cybersecurity/comptia-security-plus/practice-test) · 🎯 [Mock Exam](https://edureify.com/certification/cybersecurity/comptia-security-plus/mock-exam) · 📊 [Readiness Test](https://edureify.com/certification/cybersecurity/comptia-security-plus/readiness-test) · 📄 [Cheat Sheet](https://edureify.com/certification/cybersecurity/comptia-security-plus/cheat-sheet) · 📖 [Study Guide](https://edureify.com/certification/cybersecurity/comptia-security-plus/study-guide)

- **18%** weighting — the "think like a designer, not just a defender" domain, and a strong source of performance-based (drag-and-drop) questions

## 3.1 Compare and contrast security implications of different architecture models

- **Cloud**: shared responsibility model (provider vs. customer obligations shift by IaaS/PaaS/SaaS) and hybrid deployments
- **Infrastructure as Code (IaC)**: defining infrastructure via version-controlled config/scripts — enables consistent, auditable, repeatable deployments, but a flaw in the template propagates everywhere it's used
- **Serverless and microservices**: provider-managed runtime and independently deployed small services, respectively — shift security focus toward code-level and API-level controls
- **Network infrastructure options**: air-gapped (physically isolated), logical segmentation, and Software-Defined Networking (SDN)
- **On-premises vs. centralized vs. decentralized**: trade-offs in control, cost, and single-point-of-failure risk
- **Containerization vs. virtualization**: containers share a host kernel (lighter, but weaker isolation than VMs); VMs offer stronger isolation at higher resource cost
- **IoT, ICS/SCADA, RTOS, and embedded systems**: typically resource-constrained, hard to patch, and often prioritize availability/safety over confidentiality — usually protected via network isolation rather than traditional endpoint controls
- Evaluate each model against: availability, resilience, cost, patch availability, and risk transference (how much risk shifts to a cloud/vendor partner)

## 3.2 Given a scenario, apply security principles to secure enterprise infrastructure

- **Security zones**: logically separating network segments by trust level (e.g., DMZ vs. internal network)
- **Device placement and attributes**: active vs. passive devices, inline vs. tap/span port monitoring — inline devices can block traffic in real time but add a potential failure point; tap-based monitoring is non-disruptive but detection-only
- **Firewall types**: packet-filtering, stateful, next-generation (NGFW), and web application firewalls (WAF) each operate at different depths of inspection
- **IDS/IPS placement**: IDS detects and alerts; IPS detects and actively blocks — placement (inline vs. out-of-band) determines which is possible
- **Jump servers, proxies, load balancers**: jump servers provide a controlled, audited path to sensitive network segments; proxies mediate/filter traffic; load balancers distribute traffic for availability and can also terminate TLS
- **VPN, SD-WAN, SASE**: VPNs secure point-to-point/remote connections; SD-WAN optimizes and secures WAN traffic across multiple links; SASE (Secure Access Service Edge) converges networking and security into a cloud-delivered service for distributed workforces
- This objective is prime performance-based-question material — expect topology-placement exercises, not just definitions

## 3.3 Compare and contrast concepts and strategies to protect data

- **Data types**: regulated (e.g., healthcare, financial data subject to specific law), trade secret, intellectual property — each may carry different legal handling obligations
- **Classifications**: public through critical/restricted — mirrors the classification concept found across most security frameworks
- **Data states**: at rest, in transit, in use — each state needs a different primary control (storage encryption, TLS, and increasingly confidential-computing techniques, respectively)
- **Protection methods**: encryption, hashing (integrity, not confidentiality), masking (hiding part of a value, e.g., a credit card number), tokenization (replacing sensitive data with a non-sensitive substitute that maps back via a secure lookup), obfuscation, segmentation, and permission restrictions
- **Geographic considerations**: data sovereignty — data may be subject to the laws of the country where it's physically stored, a growing factor in cloud region selection

## 3.4 Explain the importance of resilience and recovery in security architecture

- **High availability techniques**: load balancing and clustering keep services running through individual component failure
- **Site considerations**: hot (fully ready, near-instant failover, most expensive), warm (partially ready), cold (basic infrastructure only, slowest/cheapest) recovery sites
- **Platform diversity and multi-cloud**: reduces single-vendor/single-technology risk, at the cost of added operational complexity
- **Testing approaches**: tabletop exercises (discussion-based), failover tests, and full simulations — validate that RTO/RPO assumptions actually hold in practice
- **Backup strategy**: onsite vs. offsite, frequency, encryption of backup data itself, snapshots (point-in-time captures), and journaling (continuous change logging for finer-grained recovery points)
- **Power resilience**: UPS (short-term bridge power) and generators (sustained backup power) protect availability during outages
