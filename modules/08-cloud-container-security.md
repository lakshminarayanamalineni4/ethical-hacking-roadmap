# Module 8 — Cloud and container security

**Weeks:** 20–21  
**Outcome:** Apply least privilege and secure network, storage, logging and container configuration in a test environment.

| ID | Submodule | Concepts |
|---|---|---|
| 8.1 | AWS shared responsibility | What AWS secures vs customer configuration; account hygiene |
| 8.2 | IAM | Users, roles, policies, trust policies, least privilege, MFA, access keys and rotation |
| 8.3 | VPC and network controls | Public/private subnets, route tables, security groups, NACLs, VPC endpoints |
| 8.4 | Storage and data protection | S3 Block Public Access, bucket policies, encryption, lifecycle and access logging |
| 8.5 | Monitoring and audit | CloudTrail, CloudWatch, security findings, alerting and incident evidence |
| 8.6 | Docker security | Non-root user, minimal images, pinned versions, read-only filesystem, capabilities, secrets and image scanning |
| 8.7 | CI/CD and dependencies | Dependency pinning, vulnerability scanning, secret scanning, artifact provenance |

## Practical work
- Use a dedicated test AWS environment, enable MFA, set billing alerts and avoid creating public resources.
- Review a test IAM policy and reduce permissions to the minimum needed.
- Create a private test bucket and verify public access is blocked.
- Run a local Docker container as non-root; inspect exposed ports, mounts and environment variables.
- Engineering link: secure deployment secrets, CI/CD, container images, S3 document storage, model-provider credentials and vector DB network access.

## Exit criteria
Explain IAM role trust vs permissions, identify risky exposure and implement basic container/cloud hardening.