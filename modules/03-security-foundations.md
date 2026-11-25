# Module 3 — Security foundations

**Weeks:** 6–7  
**Outcome:** Explain core security principles and implement basic defensive controls.

| ID | Submodule | Concepts |
|---|---|---|
| 3.1 | CIA triad and risk | Confidentiality, integrity, availability; assets, threats, vulnerabilities, likelihood and impact |
| 3.2 | Threat modeling | Trust boundaries, data flows, attacker goals, abuse cases, STRIDE as a structured prompt |
| 3.3 | Identity and access | Authentication vs authorization, MFA, RBAC/ABAC, least privilege, service identities |
| 3.4 | Cryptography | Encoding vs encryption vs hashing, symmetric/asymmetric crypto, keys, TLS, certificates |
| 3.5 | Password and secret storage | Argon2id/bcrypt, salts, secret managers, rotation, avoiding secrets in source/logs |
| 3.6 | Sessions and tokens | Cookies, session IDs, JWT structure, expiry, refresh, revocation, secure cookie flags |
| 3.7 | Secure error handling | Validation, safe errors, audit logging, sensitive-data minimization |

## Practical work
- Hash a sample string with SHA-256; compare with Argon2id password hashing and explain why they differ.
- Implement password hashing and verification in a local demo; never store plaintext passwords.
- Threat-model a login + password reset + JWT-protected API.
- Engineering link: map secrets and identities for FastAPI, database, vector store and model provider; inspect logs for tokens/sensitive prompts.

## Exit criteria
Threat-model a small API, explain password hashing vs encryption, and identify where secrets and authorization checks belong.