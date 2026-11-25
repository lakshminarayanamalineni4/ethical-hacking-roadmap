# Module 6 — API security

**Weeks:** 14–16  
**Outcome:** Build and assess a small API with robust identity, object-level authorization and safe operational controls.

| ID | Submodule | Concepts |
|---|---|---|
| 6.1 | API design and attack surface | REST methods, routes, schemas, OpenAPI, versioning, error behavior, exposed docs |
| 6.2 | Authentication | Password login, OAuth2 concepts, JWT validation, issuer/audience, expiry, key handling |
| 6.3 | Authorization | RBAC, ownership checks, tenant isolation, BOLA, function-level authorization |
| 6.4 | Input and output validation | Pydantic schemas, type/length/range validation, mass assignment, response filtering |
| 6.5 | Abuse controls | Rate limiting, quotas, pagination limits, request size limits, timeouts |
| 6.6 | API data protection | TLS, sensitive fields, logging redaction, idempotency, replay considerations |
| 6.7 | API testing | Positive/negative tests, role matrix, schema fuzzing in a lab, security regression tests |

## Practical work
- Build a local FastAPI + PostgreSQL service with two users and an admin role.
- Write tests proving User A cannot read/update/delete User B's objects and a normal user cannot invoke admin actions.
- Test missing, malformed, expired and wrongly scoped tokens; verify safe rejection.
- Engineering link: apply the same authorization model to chat history, uploaded files, RAG documents, vector-search filters and tool/function endpoints. A user must never retrieve another tenant's data.

## Exit criteria
Produce an authorization matrix and automated tests for user, admin and tenant boundaries.