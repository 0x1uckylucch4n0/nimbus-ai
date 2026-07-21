# Security

## Reporting
Email security@nimbus.ai. We respond within 1 business day.

## Access control
- SSO + MFA enforced on all systems (Google Workspace, GitHub, AWS).
- Production access via bastion only; least-privilege IAM.
- Offboarding: access revoked within 1 business day of termination (see `docs/offboarding.md`).

## Data
- Customer data encrypted at rest (AES-256 / KMS) and in transit (TLS 1.2+).
- Environments segregated: prod / staging / dev, no peering into production.
