# Module 4 — Reconnaissance and scanning

**Weeks:** 8–9  
**Outcome:** Inventory hosts/services in an explicitly authorized lab and interpret findings accurately.

| ID | Submodule | Concepts |
|---|---|---|
| 4.1 | Scope and rules of engagement | Written permission, target list, exclusions, test window, rate limits, stop conditions |
| 4.2 | Asset discovery | Host discovery, local network inventory, DNS records in owned/test domains |
| 4.3 | Port scanning | TCP connect scans, port states, timing, false positives and limitations |
| 4.4 | Service identification | Service/version detection, banners, service exposure and validation |
| 4.5 | Vulnerability assessment | CVE/CVSS, affected versions, exploitability vs risk, verification |
| 4.6 | Evidence and reporting | Reproducible commands, timestamps, screenshots, impact, remediation, retest |

## Practical work
- Scan 127.0.0.1 and a deliberately created local lab VM/container only; compare before/after service changes.
- Read Nmap documentation and understand options; do not blindly copy aggressive scan commands.
- Create an asset/port inventory and identify services that should not be exposed.
- Engineering link: inventory development services (API, database, Redis, vector DB, admin ports) and verify only intended interfaces are reachable.

## Exit criteria
Define scope, scan a lab target, interpret open/closed/filtered results and write a concise finding without overstating risk.

**Safety:** Never scan public IPs, employer systems, coworkers' devices or third-party services without explicit written authorization.