# Module 5 — Web application security

**Weeks:** 10–13  
**Outcome:** Identify common web risks in a training app, explain impact and implement secure fixes.

| ID | Submodule | Concepts |
|---|---|---|
| 5.1 | Web architecture and trust boundaries | Browser, frontend, backend, reverse proxy, database, cookies, CORS, same-origin policy |
| 5.2 | Broken access control | IDOR/BOLA, privilege escalation, role checks, tenant isolation, server-side authorization |
| 5.3 | Injection and SQL injection | Unsafe query construction, parameterized queries, ORM pitfalls, input handling |
| 5.4 | Cross-site scripting | Stored/reflected/DOM XSS, output encoding, sanitization, Content Security Policy |
| 5.5 | CSRF and browser controls | CSRF conditions, anti-CSRF tokens, SameSite cookies, Origin checks |
| 5.6 | Authentication and sessions | Login/reset flows, brute-force defenses, session expiry, secure cookie settings |
| 5.7 | Path traversal and file handling | Path normalization, allowlists, upload validation, storage outside web root |
| 5.8 | SSRF and security configuration | Outbound request restrictions, metadata-service protections, safe defaults, headers |
| 5.9 | Security testing workflow | Proxy traffic, reproduce in lab, capture evidence, fix, retest |

## Practical work
- Run OWASP Juice Shop locally in Docker and use its training challenges; bind to localhost or an isolated lab network.
- Use Burp Suite Community to inspect your own browser traffic to the local lab.
- For selected issues, reproduce only in the lab, explain root cause, apply a defensive fix in a toy app and add a regression test.
- Engineering link: review FastAPI routes for authorization on every object access; use parameterized SQL; validate uploads; configure CORS deliberately; do not trust frontend-only checks.

## Exit criteria
Safely demonstrate at least four web vulnerability classes in a local training app, implement fixes and write regression tests.