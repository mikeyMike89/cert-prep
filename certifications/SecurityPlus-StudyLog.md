## 2025-11-09
- Sections: 1.1 Security Controls; 1.2 CIA Triad (Messer SY0-701)
- Practice: 22 / 27 correct
- Focus for review: mapping control categories to examples; integrity mechanisms (hashing, digital signatures)

## 2025-11-10
Topics: 1.3 Change Management; 1.4 Crypto (encrypting data, key exchange, encryption tech)
- Practice: 24 / 25 correct
- Notes:
  - Standard vs. Normal vs. Emergency: clear.
  - TLS flow locked in: asymmetric for key establishment → symmetric for data.
  - Hash vs. encrypt vs. HMAC distinctions are solid.

## 2025-11-11
Topics: 1.4 Cryptography (PKI lifecycle; TLS handshake; certificates; CRL vs. OCSP; key escrow vs. backup; hashing/signatures)
- Practice: — (videos only)
- Notes:
  - TLS/ECDHE → symmetric session key flow is solid.
  - Digital signatures = hash + private key; verify with sender’s public key.
  - Quick refresh needed: CRL vs. OCSP (+stapling) and escrow vs. backup.

## 2025-11-12
Topics: 2.1-2.2 Threat Actors & Attack Vectors (threat actor types/motivations; social engineering; phishing variants; reconnaissance types)
- Practice: 19/22 correct (86%)
- Notes:
  - Active recon = direct system touching (scans); Passive/OSINT = public info gathering
  - BEC = impersonating exec for fraud; Whaling = targeting exec as victim
  - Threat actor pairing: Nation-state → APT/persistence; Script kiddie → pre-made tools
  - Solid on: vishing, smishing, pretexting, watering holes

## 2025-11-14
Topics: 2.3 Security Vulnerabilities (memory attacks; injection attacks; race conditions; system vulns; mobile/cloud/virtualization)
- Practice: ExamCompass 75% → Custom drills 87% → EOL/EOS focus 90%
- Notes:
  - Memory attacks: Injection = process manipulation; Buffer overflow = boundary violation; DLL injection = library execution
  - Critical distinctions: EOL = no free patches (paid extended possible); EOS = completely dead; Misconfiguration ≠ vulnerability
  - XSS = malicious script in trusted site; CSRF = forge requests using victim's session (actually in 3.2)
  - VM escape = breaking hypervisor boundary (real attack, not theoretical)
  - Mobile: Sideloading (unofficial sources); Jailbreak (iOS); Root (Android)
  - Solid on: SQL injection, buffer overflow, race conditions, zero-day concept
  - Weak → Strong: EOL/EOS terminology, misconfiguration identification

## 2025-11-16
Topics: 2.5 Security Techniques (segmentation/access control; mitigation techniques; hardening techniques)
- Practice: Custom Quiz 80%
- Notes:
  - Segmentation: VLANs = logical separation; DMZ = isolated network zone; Microsegmentation = software-defined boundaries
  - Hardening: Disable unnecessary services/ports = reduce attack surface; ≠ patching (which fixes vulnerabilities)
  - Mitigation types: Patching = known vulnerabilities; Hardening = attack surface reduction
  - Access controls barely touched in Messer 2.5 (more in other sections)
  - Critical finding: Messer covers ~60% of exam content
  - Solid on: Network segmentation, basic hardening concepts
  - Weak → Need work: CompTIA terminology variations, vendor-specific implementations, legacy concepts not in Messer

## 2025-11-17
Topics: 3.1 Cloud and Network Infrastructures, Concepts and Considerations
- Practice: 17/20 correct (85%)
- Notes:
  - Cloud Models & Services: IaaS, PaaS, SaaS → Responsibility matrix defines who manages what (varies by provider and service model)
    - Infrastructure as Code (IaC) - Infrastructure managed entirely through code/definition files
    - Serverless - Server exists but customer doesn't manage it
  - Architecture Types:
    - Monolithic - Single large application; challenges with codebase size and change control
    - Microservices - APIs connect independent services; provides scalability, resilience, and built-in containment
  - Network Infrastructure:
    - Physical isolation (air-gapped) vs logical isolation (VLANs)
    - Software-Defined Networking (SDN) - Simplifies administration and troubleshooting
    - On-premises vs cloud-based; centralized vs decentralized
  - System Types:
    - Virtualization vs containerization
    - SCADA/ICS, RTOS, Embedded systems
    - High availability considerations
  - Key Distinctions:
    - Scalability - Ability to scale resources up/down as needed
    - Elasticity - Infrastructure automatically scales based on demand
  - Weaknesses:
    - IaaS vs PaaS vs SaaS differences → Create comparison chart
    - IaC security concerns → Research hardcoded credential risks
