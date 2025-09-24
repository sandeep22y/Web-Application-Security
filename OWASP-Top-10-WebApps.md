# OWASP Top 10 for Application Security (2021)  
This document lists the OWASP Top 10 application security risks along with brief recommendations for mitigation.

| **ID** | **Risk** | **Description** | **Recommendations / Mitigations** |
|--------|-----------|-----------------|-----------------------------------|
| **A01:2021** | Broken Access Control | Weak or missing enforcement of access controls allows attackers to act outside their intended permissions. | • Enforce server-side access control checks<br>• Deny by default and least-privilege access<br>• Implement role-based access controls (RBAC) and test frequently |
| **A02:2021** | Cryptographic Failures (formerly Sensitive Data Exposure) | Improper use of cryptography leads to exposure of sensitive data in transit or at rest. | • Use strong, industry-standard encryption (TLS 1.2+, AES-256)<br>• Disable weak ciphers and protocols<br>• Do not store sensitive data unless necessary; encrypt at rest |
| **A03:2021** | Injection | Untrusted data is sent to an interpreter as part of a command or query, tricking the interpreter into executing unintended commands. | • Use parameterized queries/prepared statements<br>• Validate and sanitize input<br>• Employ ORM frameworks to reduce direct query building |
| **A04:2021** | Insecure Design | Design flaws leave applications vulnerable regardless of implementation correctness. | • Perform threat modeling during design<br>• Use secure design patterns and reference architectures<br>• Incorporate security requirements early in SDLC |
| **A05:2021** | Security Misconfiguration | Insecure default configurations, incomplete or ad-hoc configurations. | • Harden server and application configurations<br>• Disable default accounts, sample apps, unnecessary services<br>• Automate configuration management and use CIS benchmarks |
| **A06:2021** | Vulnerable and Outdated Components | Using components with known vulnerabilities. | • Maintain an inventory (SBOM) of components<br>• Regularly scan for vulnerabilities (e.g., SCA tools)<br>• Apply timely security patches and updates |
| **A07:2021** | Identification and Authentication Failures | Weak or misconfigured authentication mechanisms. | • Enforce MFA wherever possible<br>• Store passwords securely (bcrypt/Argon2)<br>• Implement lockouts, session timeouts, and secure cookie handling |
| **A08:2021** | Software and Data Integrity Failures | Code and data integrity is not verified, leading to unauthorized changes. | • Use digital signatures and checksums<br>• Verify updates, plugins, libraries before use<br>• Employ CI/CD integrity controls |
| **A09:2021** | Security Logging and Monitoring Failures | Insufficient logging and monitoring prevents timely detection of breaches. | • Implement centralized logging and SIEM<br>• Log authentication failures, access control failures, and server errors<br>• Establish and test an incident response process |
| **A10:2021** | Server-Side Request Forgery (SSRF) | Applications fetch remote resources without validating user-supplied URLs, enabling attackers to target internal systems. | • Validate and sanitize all URLs before requests<br>• Enforce allow-lists for remote destinations<br>• Isolate SSRF-prone services in network segments |

> 📌 *This table summarizes the key application security risks identified by OWASP and recommended mitigations to reduce exposure.*


<img width="936" height="258" alt="image" src="https://github.com/user-attachments/assets/76f2c00a-0814-4e47-933e-db458ff5b278" />




