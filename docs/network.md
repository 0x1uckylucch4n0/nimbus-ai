# Network

- **Production boundary**: public internet terminates at the ALB (:443 only).
- **Private subnet**: ECS api, RDS `prod-db` (encrypted), S3 `uploads` (SSE-KMS). No public ingress.
- **Segregation**: staging (synthetic data) and dev carry no data stores and do not peer into production.
- **Admin access**: bastion host, SSO + MFA only.

Manifest generates the labeled audit diagram from live AWS config.
