## Password Managers — By Umbra

## Bitwarden
 
- **Official Website:** https://bitwarden.com/
- **Open Source:** Yes — https://github.com/bitwarden
- **Storage:** Cloud-based, with self-hosting options
- **End-to-End Encryption (E2EE):** Yes
- **Security Model:** Zero-Knowledge architecture; vault data is encrypted before being sent to the server.
- **Platforms:** Windows, macOS, Linux, Android, iOS, Web, and browser extensions
- **Independent Security Audits:** Yes
- **Last Reviewed:** 2026-10-20

 
### Strengths
 
- **Open Source:** Its source code is publicly available for inspection and contributions. However, open source alone does not guarantee the absence of vulnerabilities.
- **Strong Encryption:** Vault data is encrypted according to Bitwarden's published security architecture, limiting the provider's ability to access users' stored secrets.
- **Independent Security Audits:** The company publishes information about third-party security assessments and penetration tests.
- **Cross-Platform Synchronization:** Users can access their vaults across multiple operating systems and devices.
- **Self-Hosting Support:** Technically experienced users can operate their own server for greater control over the hosting environment.
- **Security Features:** Includes password generation, multi-factor authentication, secure sharing, and password health tools.

 
### Weaknesses and Risks
 
- **Master Password Dependency:** Losing the master password may result in permanent loss of access if no suitable recovery method is available.
- **Compromised Devices:** Malware, keyloggers, or malicious browser extensions may expose passwords after they are decrypted on the user's device.
- **Phishing Attacks:** A password manager does not prevent every phishing attack, particularly when users enter credentials on fraudulent websites.
- **Self-Hosting Complexity:** Users are responsible for server updates, hardening, backups, access control, and ongoing security maintenance.
- **Browser and Autofill Risks:** Vulnerabilities in browsers, extensions, or autofill behavior may expose credentials under certain conditions.
- **Open Source Is Not a Guarantee:** The software can still contain vulnerabilities, making regular updates and security advisories important.

 
### Has Bitwarden Ever Been Hacked?
 
 
- **Confirmed server breach or vault data leak:** Based on the sources listed below, I could not verify a confirmed incident involving a breach of Bitwarden's servers that exposed users' vaults. On February 16, 2026, Bitwarden stated that it had not experienced a security breach. This reflects publicly available information and the company's statement, not proof that no undisclosed incident has ever occurred.
 
- **2026 — ETH Zurich Cryptography Assessment:** A security assessment examined cryptographic design and scenarios involving a potentially malicious server. This was a security evaluation, not evidence of an actual server compromise.
   
  - **Source:** https://bitwarden.com/blog/security-through-transparency-eth-zurich-audits-bitwarden-cryptography/
 
- **2023 — Autofill Security Research:** Google Security Research published research concerning autofill behavior in several password managers, including a specific Bitwarden version. This concerned a security vulnerability or behavior in a particular version; it was not evidence of a server breach or a database leak.
   
  - **Source:** https://github.com/google/security-research/security/advisories/GHSA-mhhf-w9xw-pp9x
 

 
### Security References
 
- **Security White Paper:** https://bitwarden.com/help/bitwarden-security-white-paper/
- **Encryption Protocols:** https://bitwarden.com/help/what-encryption-is-used/
- **Independent Audits:** https://bitwarden.com/help/is-bitwarden-audited/
- **Official Source Code:** https://github.com/bitwarden

 
### Overall Assessment
 
Bitwarden is a strong option for users seeking an open-source password manager with cross-platform synchronization, end-to-end encryption, and self-hosting capabilities.
 
Its main risks involve compromised user devices, phishing, master password loss, and the operational burden of self-hosting. Users should employ a strong, unique master password, enable multi-factor authentication, keep applications updated, and maintain secure recovery procedures.
 
**Security Verdict:** A strong candidate for personal and organizational use, provided users maintain good security practices and keep their software up to date.

___

## Proton Pass

- **Official Website:** https://proton.me/pass
- **Open Source:** Yes — https://github.com/ProtonPass
- **Storage:** Cloud-based, with end-to-end encrypted synchronization. No standard self-hosting option.
- **End-to-End Encryption (E2EE):** Yes
- **Security Model:** Zero-knowledge architecture. Vault data is encrypted on the user's device before synchronization with Proton's servers.
- **Platforms:** Windows, macOS, Linux, Android, iOS, Web, browser extensions, and CLI.
- **Independent Security Audits:** Yes — Cure53 (2023) and Recurity Labs (2026).
- **Last Reviewed:** 2026-10-20

### Strengths

- **Open Source:** Publicly available source code allows researchers to inspect the implementation. However, open source does not guarantee the absence of vulnerabilities.
- **Strong Encryption:** Uses AES-256-GCM for vault data encryption, according to Proton's published security documentation.
- **Independent Security Audits:** Proton Pass has undergone independent assessments, including Cure53 in 2023 and Recurity Labs in 2026.
- **End-to-End Encrypted Synchronization:** Vault contents are encrypted so the provider cannot ordinarily read their plaintext contents.
- **Cross-Platform Support:** Supports major desktop and mobile platforms, web access, and browser extensions.
- **Security Features:** Includes password generation, passkey management, secure sharing, two-factor authentication support, and hide-my-email aliases. Availability may vary by plan.
- **Public Bug Bounty Program:** Security researchers can report vulnerabilities through Proton's responsible disclosure process.

### Weaknesses and Risks

- **Account Recovery Dependency:** Losing access to the account or necessary recovery information may make it difficult or impossible to restore access.
- **Compromised Devices:** Malware, keyloggers, and malicious extensions may expose credentials after they are decrypted on the device.
- **Phishing Attacks:** A password manager does not eliminate phishing or guarantee that users will avoid fraudulent websites.
- **Cloud Service Dependency:** Hosted synchronization depends on Proton's infrastructure and service availability.
- **No Primary Self-Hosting Option:** Proton Pass is primarily a managed cloud service, which may not suit users who require complete control over server infrastructure.
- **Browser and Autofill Risks:** Vulnerabilities in extensions, browsers, or autofill behavior can expose credentials in certain circumstances.
- **Open Source Is Not a Guarantee:** Public code can still contain implementation flaws, dependency vulnerabilities, and configuration errors.
- **Third-Party Trust and Account Security:** Security also depends on account authentication, recovery procedures, device security, and correct implementation of cryptographic protocols.

### Has Proton Pass Ever Been Hacked?

- **Confirmed server breach or vault data leak:** I could not verify a publicly confirmed incident in the sources reviewed in which attackers breached Proton Pass servers and exposed users' decrypted vault contents. This is not proof that no undisclosed incident has ever occurred.

- **2026 — Recurity Labs Security Audit:** Proton announced an independent assessment conducted between January and April 2026, covering browser extensions, mobile and desktop applications, and the command-line interface. This was a security assessment, not evidence of an actual server breach.
- **Source:** https://proton.me/business/blog/proton-pass-audit-2026

- **2025 — Clickjacking Vulnerability:** Proton reported a clickjacking vulnerability affecting its web application and stated that it was addressed in version 1.31.6. This was an application-level vulnerability, not evidence of a server compromise or a confirmed mass vault-data leak.
- **Source:** https://proton.me/blog/proton-pass-is-protected-against-clickjacking-attacks

- **2023 — Cure53 Security Audit:** Cure53 assessed Proton Pass's mobile applications, browser extensions, and API. Proton published information about the findings and remediation status. An audit finding is not, by itself, evidence of an actual attack.
- **Source:** https://proton.me/blog/pass-open-source-security-audit

**Important distinction:** A security audit or vulnerability report does not prove that an attacker exploited the issue, stole data, or compromised the provider's servers. Likewise, the absence of a publicly confirmed server breach does not prove that a service is invulnerable.

### Security References

- **Official Website:** https://proton.me/pass
- **Security Overview:** https://proton.me/pass/security
- **Security Model and Encryption Design:** https://proton.me/blog/proton-pass-security-model
- **Independent Security Audit (2023):** https://proton.me/blog/pass-open-source-security-audit
- **2026 Recurity Labs Audit:** https://proton.me/business/blog/proton-pass-audit-2026
- **Clickjacking Vulnerability and Fix:** https://proton.me/blog/proton-pass-is-protected-against-clickjacking-attacks
- **Official Source Code:** https://github.com/ProtonPass

### Overall Assessment

Proton Pass is a strong option for users seeking an open-source password manager with end-to-end encryption, cross-platform synchronization, and independently assessed security controls.

Its published encryption model, public source code, security audits, and vulnerability disclosure program provide meaningful security assurances. However, these measures do not eliminate vulnerabilities or risks from compromised devices, phishing, account recovery problems, or browser extensions.

Users should employ a strong, unique account password, enable two-factor authentication, keep applications updated, secure their recovery methods, and maintain a secure backup or export where appropriate.

**Security Verdict:** Proton Pass is a strong candidate for personal and organizational password management, particularly for users who prioritize end-to-end encryption, open-source transparency, and cross-platform access. Its security depends on both its technical design and the user's security practices.

___
## KeePass

- **Official Website:** https://keepass.info/
- **Open Source:** Yes — https://sourceforge.net/projects/keepass/
- **Storage:** Local encrypted database file (KDBX for KeePass 2.x). Users can manually synchronize or back up the database using their preferred storage service.
- **End-to-End Encryption (E2EE):** Not applicable in the traditional cloud-sync sense. KeePass encrypts the database locally before it is stored or transferred.
- **Security Model:** Local-first, offline-capable password management. The database is protected by a master key that can combine a master password, key file, and Windows user account key.
- **Platforms:** Official KeePass 2.x primarily supports Windows. KeePass 2.x may run on other platforms with compatible runtimes; third-party ports are available for mobile and other operating systems.
- **Independent Security Audits:** Publicly documented security research and vulnerability assessments exist. Do not assume every release has undergone a comprehensive independent audit.
- **Last Reviewed:** 2026-10-20

### Strengths

- **Open Source:** KeePass is free and open source, allowing its source code to be inspected and independently reviewed.
- **Strong Encryption:** KeePass 2.x supports AES-256 and ChaCha20 for database encryption. KeePass 1.x supports AES-256 and Twofish.
- **Local Storage and Privacy:** The database is stored as an encrypted file under the user's control. KeePass does not require a vendor-operated cloud account or centralized synchronization server.
- **Multiple Key Components:** Users can combine a master password with a key file or a Windows user account key, adding protection when configured correctly.
- **Protection Against Password Guessing:** Key derivation functions such as AES-KDF and Argon2 in KeePass 2.x increase the computational cost of guessing a weak master password.
- **Offline Availability:** Users can access their password database without an internet connection, provided the application and database are available locally.
- **Portable Use:** KeePass can be run in portable configurations, making it possible to carry an encrypted database and application between compatible systems.
- **Security Controls:** Includes automatic locking, clipboard clearing options, secure desktop support for entering the master key, password generation, and process-memory protections with documented limitations.
- **No Mandatory Cloud Subscription:** The core application is free, and users choose how to back up or synchronize the encrypted database.

### Weaknesses and Risks

- **Master Password Dependency:** Losing the master password or another required key component can result in permanent loss of access to the database. KeePass does not provide a universal recovery key.
- **Compromised Devices:** Malware, keyloggers, screen capture tools, or spyware may capture passwords when the database is open or credentials are entered.
- **Manual Synchronization:** Users must arrange synchronization and backups themselves. Poorly managed copies may become outdated, conflict, or be lost.
- **Key File Management:** Losing a required key file can make the database inaccessible. Storing the key file alongside the database may reduce the security benefit if both are stolen together.
- **Plugin Risks:** Third-party plugins can expand functionality but may introduce vulnerabilities or access sensitive information. Only install trusted, necessary plugins.
- **Autofill and Auto-Type Risks:** Automated typing and integration with other applications can expose credentials if the wrong window or website is targeted.
- **Open Source Is Not a Guarantee:** Source availability does not eliminate implementation flaws, malicious modifications, or vulnerabilities in dependencies.
- **Port and Compatibility Differences:** Third-party mobile and cross-platform implementations may have different features, release schedules, and security properties from the official Windows application.
- **Local Backup Security:** Copies of the encrypted database may be exposed to offline password-guessing attempts if an attacker obtains them. A weak master password increases this risk.
- **No Centralized Recovery or Administration by Default:** Organizations may need additional tools and procedures to manage access, backups, updates, and recovery across multiple users.

### Has KeePass Ever Been Hacked?

- **Confirmed centralized server breach or cloud vault leak:** KeePass is primarily a local password manager and does not operate a mandatory centralized vault synchronization server. I could not verify a publicly confirmed incident involving a breach of an official KeePass cloud vault service exposing users' databases. This does not prove that every KeePass installation, third-party port, plugin, or user's device has always been secure.

- **2026 — CVE-2026-86776 / Database Header Memory Allocation:** KeePass's official security-issues page discusses a report concerning memory allocation when processing a KDBX database header. The project maintainer disputes the claim that this behavior constitutes a security vulnerability, explaining that the file format permits large header fields and that the application validates the field size. This is a disputed security report, not evidence of a confirmed password theft or database breach.
- **Source:** https://keepass.info/help/kb/sec_issues.html

- **Historical — KDB/KDBX Header Authentication Issues:** Research into password-manager database formats identified weaknesses involving unauthenticated database headers, including possible silent data removal or corruption in older formats and versions. KeePass introduced header authentication in KeePass 1.24 and 2.20 to address these issues. The published analysis stated that confidentiality was not compromised by these particular attacks.
- **Source:** https://keepass.info/help/kb/sec_issues.html

- **Historical — KeeFarce and Running-Process Extraction:** The KeeFarce tool demonstrated that an attacker with sufficient access to a running KeePass process could extract data from an unlocked database. The KeePass maintainer explains that this reflects the broader limitations of defending an application against spyware running with the same user's privileges, rather than a remote attack against an encrypted database server.
- **Source:** https://keepass.info/help/kb/sec_issues.html

- **2022 — CVE-2022-0725:** A security issue involving sensitive data in Fedora system logs was listed in KeePass's official security-issues documentation. This is a specific logging issue and should not be described as a breach of KeePass's servers or a confirmed mass disclosure of password databases.
- **Source:** https://keepass.info/help/kb/sec_issues.html

**Important distinction:** KeePass vulnerabilities, weaknesses in older versions, malicious plugins, and attacks against compromised computers are not equivalent to a breach of a centralized KeePass server. Because KeePass is local-first, the relevant security questions include database encryption, the strength of the master key, application integrity, and the security of the device that opens the database.

### Security References

- **Official Website:** https://keepass.info/
- **Security Documentation:** https://keepass.info/help/base/security.html
- **Official Security Issues List:** https://keepass.info/help/kb/sec_issues.html
- **Master Key Documentation:** https://keepass.info/help/base/keys.html
- **Database Settings and Key Derivation:** https://keepass.info/help/v2/dbsettings.html
- **Official Release History:** https://keepass.info/news/news_all.html
- **Official Source Code / Project:** https://sourceforge.net/projects/keepass/
- **KeePass 2.x File Format Specification:** https://keepass.info/help/kb/kdbx.html

### Overall Assessment

KeePass is a strong option for users who prefer local password storage, open-source software, offline access, and direct control over their encrypted database files. Unlike cloud-first password managers, it does not require a provider-operated synchronization service to store and open the vault.

Its security depends heavily on the strength of the master password, appropriate key-derivation settings, careful handling of any key files, trusted application downloads, and protection of the device while the database is unlocked. Users who synchronize the database through a cloud storage provider should remember that the provider stores a copy of the encrypted file and that synchronization and recovery are their responsibility.

Users should create a strong and unique master passphrase, consider Argon2 for KeePass 2.x where supported by their clients, keep the application and trusted ports updated, avoid unnecessary plugins, enable automatic locking, and maintain tested backups of the encrypted database. Key files should be backed up securely and stored separately from the database where practical.

**Security Verdict:** KeePass is a strong candidate for users who prioritize local control, offline functionality, and open-source transparency. Its lack of a mandatory cloud service reduces dependence on a centralized provider, but places greater responsibility on users to protect devices, manage keys, maintain backups, and secure any synchronization process.

___
