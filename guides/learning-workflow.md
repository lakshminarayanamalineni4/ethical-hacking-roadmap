# Learning workflow

Use this for every submodule.

1. **Understand** — Read a trusted explanation. Identify what it is, why it exists, how it works and where it is used. Done when you can explain it simply without copying.
2. **Trace** — Draw the request/data flow. Mark inputs, identities, permissions, trust boundaries and failure cases. Done when you can point to where the risk/control exists.
3. **Implement** — Build a small example or configure a local lab. Where appropriate, demonstrate a weakness only in a deliberately vulnerable lab, then implement the secure fix. Done when a repeatable exercise exists.
4. **Test** — Test normal, invalid, unauthorized, boundary and failure cases. Observe responses and logs. Done when expected and unexpected behavior is demonstrated.
5. **Document** — Record finding/skill, impact, root cause, sanitized evidence, remediation and retest result. Done when a short note/report is saved.
6. **Revise** — Recall without notes, redo a smaller exercise and answer review questions. Done when you can explain and perform it after a delay.

## Suggested note template
- Concept and module/submodule ID:
- Explanation in my own words:
- Why it matters:
- Request/data flow or diagram:
- Threats / failure cases:
- Lab setup and authorized scope:
- Steps performed:
- Expected vs actual result:
- Root cause:
- Secure fix / mitigation:
- Tests and retest:
- Evidence link (sanitized):
- Questions I still have:
- Revision scores and next review:

## Evidence hygiene
Never store real secrets, access tokens, private keys, customer data, production exploit details or unredacted sensitive logs. Use synthetic accounts and disposable data.