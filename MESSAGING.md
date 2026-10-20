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

## SimpleX Chat Security Assessment

- **Official Website**: https://simplex.chat
- **Type**: Privacy-focused messenger using decentralized identity and private message-relay architecture
- **End-to-End Encryption**: Yes. SimpleX uses its own messaging protocols with Double Ratchet-based encryption and additional cryptographic protections, including post-quantum key exchange mechanisms in supported protocol versions.
- **Identity Required**: None. No phone number, email address, username, or permanent global user identifier is required. Users connect through invitation links or QR codes. Optional public addresses are available.
- **Metadata Protection**: Very High. SimpleX does not assign users global identifiers. It uses separate, unidirectional message queues and additional encryption layers to reduce the ability of servers to correlate senders and recipients. Message padding also reduces information leakage from message sizes. However, traffic timing and other metadata may still reveal information under some conditions.
- **IP Exposure**: Protected by the messaging architecture, but not completely hidden from every network participant. Messaging relay servers can observe the IP addresses of clients directly connecting to them, but the protocol's routing and encryption are designed to prevent a single relay from linking message content and both communicating parties. Tor or a VPN can provide additional network-level privacy.
- **Open Source**: Yes. SimpleX Chat clients, protocol implementations, and server components are publicly available for inspection. The project uses the AGPLv3 license for its open-source code.
- **Independent Audits**: "Trail of Bits 2022 Implementation Security Assessment" (https://simplex.chat/blog/20221108-simplex-chat-v4-2-security-audit-new-website.html) / "Trail of Bits 2024 Cryptographic Protocol Design Review" (https://simplex.chat/blog/20241014-simplex-network-v6-1-security-review-better-calls-user-experience.html). The official security policy also lists a June 2026 implementation assessment as scheduled; its completion should not be assumed without a published report.
- **Known Security Incidents**: No claim of zero historical incidents can be established from the cited sources alone. Trail of Bits identified security issues during its 2022 assessment and additional findings during its 2024 protocol review. These included issues requiring sophisticated attacks; the project reported fixing some findings and accepting others. Consult current advisories and release notes for the latest status.
- **Main Weakness**: Device compromise remains a major risk. If an attacker gains access to an unlocked device, its local chat database, or the app itself, end-to-end encryption cannot guarantee confidentiality. In addition, disabling Always use relay for audio and video calls can allow peer-to-peer connections that reveal your IP address to the other participant. Relay servers may also observe connection metadata and call duration, depending on configuration.
- **Best For**: Privacy-conscious users, journalists, activists, researchers, and people who want to communicate without linking their messaging identity to a phone number or email address. It is particularly suitable for users seeking strong metadata minimization and control over their communication infrastructure.
- **Official Documentation**: https://simplex.chat/docs/simplex.html / "Privacy and Security Guide" (https://simplex.chat/docs/guide/privacy-security.html) / "Security Policy" (https://simplex.chat/security/)
- **Sources**: SimpleX Chat technical documentation, official security policy, published Trail of Bits assessments, and official privacy and security guides.
- **Last Reviewed**: 2026-10-20

**Privacy Rating**: 9/10
**Security Rating**: 8.5/10
**Anonymity Rating**: 9/10

Ratings are subjective assessments, not official certifications or standardized measurements.

**Verdict**:

SimpleX Chat offers strong privacy-oriented messaging without requiring a phone number, email address, or permanent global user identifier. Its separate message queues, layered encryption, and metadata-minimizing design provide meaningful privacy advantages over systems built around persistent user identities. However, SimpleX is not a guarantee of complete anonymity: IP addresses may be visible to directly contacted network infrastructure, traffic analysis remains possible, and calls can expose IP addresses when peer-to-peer connections are used. Independent security assessments provide useful evidence, but they do not prove the absence of all vulnerabilities. For high-risk communications, keep the app updated, verify contact security codes, protect devices and backups, and configure call relays and network routing according to your threat model.
