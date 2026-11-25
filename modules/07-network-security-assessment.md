# Module 7 — Network security assessment

**Weeks:** 17–19  
**Outcome:** Assess a small isolated lab and validate findings without harming systems.

| ID | Submodule | Concepts |
|---|---|---|
| 7.1 | Network architecture review | Subnets, segmentation, ingress/egress, management plane, exposed services |
| 7.2 | Service and configuration review | Default credentials in lab, unnecessary services, insecure protocol/configuration concepts |
| 7.3 | Vulnerability validation | Match product/version/configuration to advisories; validate safely and avoid destructive tests |
| 7.4 | Controlled exploitation concepts | Proof-of-concept validation, impact boundaries, cleanup and stop conditions |
| 7.5 | Windows/Linux hardening | Patch management, firewall rules, account hygiene, secure remote administration |
| 7.6 | Assessment report | Severity rationale, evidence, business impact, remediation and retest |

## Practical work
- Use a purpose-built vulnerable VM from a reputable training platform on a host-only/internal virtual network.
- Enumerate only the lab VM; identify an intentionally vulnerable configuration using lab instructions.
- Apply a patch/configuration fix and repeat validation.
- Engineering link: review development/staging network exposure and create a checklist for database, cache, admin and observability endpoints.

## Exit criteria
Document a scoped network assessment and distinguish a confirmed vulnerability from an unverified scanner result.