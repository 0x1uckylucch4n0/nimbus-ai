# Nimbus AI

Cloud platform for automated infrastructure workflows.

> **Demo repository** — illustrative content for a Manifest compliance demo (SOC 2). Not production code.

## Stack
- **API**: TypeScript / Node (ECS)
- **Data**: PostgreSQL (RDS, encrypted), S3 (SSE-KMS)
- **Edge**: ALB (:443), Cloudflare
- **CI/CD**: GitHub Actions to production on merge to main
- **Identity**: Google Workspace (SSO + MFA), Rippling (HRIS)
- **Tickets**: Jira (OPS project)

## Compliance
Manifest is our AI compliance officer. It reads this repo and our stack read-only to draft policies, capture evidence, and keep us audit-ready. See SECURITY.md.
