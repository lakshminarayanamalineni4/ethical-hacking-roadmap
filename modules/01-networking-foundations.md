# Module 1 — Networking foundations

**Weeks:** 1–3  
**Outcome:** Explain how a browser/API client and server communicate; inspect traffic in your own lab.

| ID | Submodule | Concepts |
|---|---|---|
| 1.1 | Network models | OSI and TCP/IP layers, encapsulation, client/server, LAN/WAN |
| 1.2 | Addressing | IPv4/IPv6, private/public IPs, loopback, MAC, subnet masks, CIDR, default gateway |
| 1.3 | Ports and protocols | TCP vs UDP, ports, sockets, common service ports, listening vs established |
| 1.4 | DNS | Resolvers, A/AAAA/CNAME/MX/TXT, recursive lookup, caching, troubleshooting |
| 1.5 | HTTP and HTTPS | Request/response, methods, status codes, headers, cookies, TLS, certificates, redirects |
| 1.6 | Routing and network controls | Routing, NAT, VPN, firewall, security groups, segmentation |
| 1.7 | Packet analysis | Wireshark filters, DNS/TCP handshake, TLS visibility limits, capture ethics |

## Practical work
- Use PowerShell: `ipconfig`, `ping`, `nslookup`, `tracert`, `route print`, `netstat -ano`, `Test-NetConnection`.
- Capture traffic to a local test web server in Wireshark; identify DNS, TCP handshake and HTTP request/response.
- Build a simple Python HTTP client/server and inspect local traffic.
- Engineering link: trace browser → reverse proxy → FastAPI → PostgreSQL/Redis/LLM provider; identify ports and trust boundaries.

## Exit criteria
Draw and explain a complete request path; interpret basic packet captures; distinguish DNS, routing, transport and application-layer issues.