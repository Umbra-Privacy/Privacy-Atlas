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

**Privacy Rating:** 9.5/10
**Security Rating:** 9/10
**Anonymity Rating:** 10/10

**Verdict:** Session is a premier messaging tool for absolute anonymity due to its lack of phone-number ties and robust metadata protection via onion routing.

___
