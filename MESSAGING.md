# Messaging Privacy Tools – By Umbra

## Session Messenger Security Assessment

- **Official Website:** [https://getsession.org](https://getsession.org)
- **Type:** Decentralized Messenger
- **End-to-End Encryption:** Yes (Session Protocol, derived from Signal Protocol)
- **Identity Required:** None (uses a unique 66-character alphanumeric Session ID)
- **Metadata Protection:** High. No phone numbers, emails, locations, or central logs are recorded. It utilizes onion-routing paths to mask sender and receiver metadata.
- **IP Exposure:** Protected. Messages traverse a decentralized, distributed network of user-operated "Service Nodes." Individual nodes only see the IP address of the preceding node in the path, preventing any single entity from linking your IP address to your Session ID.
- **Open Source:** Yes (Clients and Service Node repository are publicly verifiable)
- **Independent Audits:** [Quarkslab 2020 Code Audit](https://getsession.orgblog/session-security-audit- Quarkslab) / [Oxen Core 2021 Security Assessment](https://oxen.io)
- **Known Security Incidents:** No Confirmed Incident Found (No infrastructure-wide database leaks or cryptographic breaches have ever been documented)
- **Main Weakness:** Voice and video calls routing through standard peer-to-peer (P2P) connections can leak IP addresses to call participants unless you explicitly turn on the "Always Relay Calls" option in settings.
- **Best For:** High-risk whistleblowers, activists, and users requiring complete identity isolation from physical SIM cards or device hardware IDs.
- **Official Documentation:** [https://oxen.io](https://oxen.io)
- **Sources:** Oxen Privacy Tech Foundation Network Specifications and Independent Cryptographic Reviews.
- **Last Reviewed:** 2026-10-20

**Privacy Rating:** 8.5/10
**Security Rating:** 8/10
**Anonymity Rating:** 8.75/10

**Verdict:**
ession offers privacy-oriented messaging without requiring a phone number or email address. Its protection depends on the threat model, device security, network conditions, and communication features used. Do not interpret pseudonymous identifiers or onion routing as guarantees of complete anonymity. Review current technical documentation, independent audits, and security advisories before relying on it for high-risk communications.

___
