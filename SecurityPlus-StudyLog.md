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
