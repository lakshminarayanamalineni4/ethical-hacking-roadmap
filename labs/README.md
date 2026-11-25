# Practical labs

Keep exercises reproducible, local and isolated wherever possible.

## Environment
- Primary: Windows 10/11 + WSL2 Ubuntu.
- Optional: Kali VM for learning tools; isolate it from production and unrelated networks.
- Containers: Docker-based local labs, ports bound to localhost unless the exercise requires otherwise.
- Targets: intentionally vulnerable training applications or systems you own and are explicitly authorized to assess.

## Lab record
For each lab, document objective, setup, authorized scope, steps, observations, expected/actual behavior, cleanup, remediation and sanitized evidence.

## Rules
Never scan or exploit public IPs, employer systems, coworkers' devices or third-party services without explicit written approval. Use synthetic accounts and disposable test data. Do not commit secrets or real customer data.