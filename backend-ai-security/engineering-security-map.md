# Security in daily Backend + AI engineering

Apply these controls proportionately during design, coding, review, testing and deployment.

| Work area | Security concepts | Practical habit |
|---|---|---|
| FastAPI/API route | Authentication, authorization, BOLA/IDOR, validation, safe errors, rate limits | Add negative tests: unauthenticated, wrong role, wrong owner/tenant, malformed input. |
| PostgreSQL/SQLAlchemy | SQL injection, least-privilege DB roles, sensitive data, backups | Use parameterized queries/ORM safely; restrict DB privileges; avoid logging secrets/personal data. |
| JWT/login/sessions | Token validation, expiry, issuer/audience, key management, password hashing, MFA | Test expired/invalid tokens and role changes; use Argon2id/bcrypt for passwords. |
| RAG ingestion/retrieval | Document ACLs, tenant isolation, prompt injection, unsafe file parsing, data leakage | Carry user/tenant ACL filters into retrieval; test cross-user retrieval; treat retrieved text as untrusted. |
| LLM prompts/tool calling | Prompt injection, excessive agency, insecure output handling, sensitive disclosure | Enforce server-side authorization for every tool action; validate structured outputs; allowlist tools and bound permissions. |
| Vector database/embeddings | Tenant filters, metadata access, deletion lifecycle, retention | Test cross-tenant isolation; verify deletion and re-indexing behavior. |
| File upload/object storage | Path traversal, malicious files, public bucket exposure, content-type trust | Validate size/type, scan where appropriate, randomize storage names, default to private. |
| Docker/local development | Root containers, exposed ports, secrets in images, unsafe mounts | Use non-root users, bind dev services to localhost, use secret management and minimal images. |
| AWS deployment | IAM least privilege, segmentation, storage permissions, audit logs | Prefer roles over long-lived keys; review security groups and S3 public-access settings. |
| CI/CD/code review | Dependency vulnerabilities, leaked secrets, unsafe artifacts, missing tests | Add approved secret/dependency scanning and security regression tests. |
| Logging/observability | Sensitive-data leakage, auditability, log injection, alerting | Redact credentials/tokens; log security-relevant events without sensitive payloads. |
| Architecture/design | Threat modeling, trust boundaries, abuse cases, data classification | Draw data flows and ask who can access, change, trigger or retrieve each resource. |

## Feature security checklist
- [ ] Identity: who is calling, and is identity verified server-side?
- [ ] Authorization: is access checked for this exact object, action and tenant?
- [ ] Input: are type, size, format and allowed values validated?
- [ ] Data: are secrets/sensitive fields protected in storage, transit, logs and responses?
- [ ] Abuse: are rate, size, time and resource limits appropriate?
- [ ] Dependencies: are packages, images and integrations maintained and reviewed?
- [ ] AI/RAG: is retrieved content treated as untrusted, and are tools permission-checked independently of the model?
- [ ] Observability: can suspicious behavior be detected without logging sensitive content?
- [ ] Tests: are unauthorized, invalid and boundary cases covered by automated tests?