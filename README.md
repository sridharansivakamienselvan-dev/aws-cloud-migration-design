# AWS Cloud Migration Design

Academic project designing a centralised AWS platform to migrate individual store databases into the cloud for a simulated UK supermarket chain.

## Status

Work in progress. This repository is being built from scratch and will hold the architecture design, migration plan, and security and cost considerations.

## Design summary

The target architecture centralises store data in Amazon RDS with Amazon S3 for object storage and backups, replacing per-store databases that were costly to maintain and difficult to report across. The design covers network layout, availability, backup and recovery expectations, and how reporting can be served from a single consistent data set.

## Security considerations

Access is scoped with least-privilege IAM roles, data is encrypted at rest and in transit, and logging and monitoring are included so that activity across the platform is auditable. Migration sequencing is planned to limit downtime for individual stores.

## Planned repository layout

Architecture diagrams and the written design will live under docs, migration runbooks under migration, and any infrastructure-as-code templates under infra.

## Note

This is an academic design exercise for a simulated organisation. No real customer data or production credentials are included.
