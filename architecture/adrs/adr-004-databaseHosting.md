## ADR 004: Database Hosting — Amazon RDS

### Context

We need a way to host and manage our PostgreSQL database in production. The hosting solution must provide reliability, backups, security, and ease of maintenance while allowing us to focus on application development.

### Options

**Amazon RDS (Managed PostgreSQL)**: Fully managed service with automated backups, patching, replication, and scaling. Higher cost but minimal ops overhead.

**Self-managed on EC2**: Full control over database configuration and cost optimization. Requires manual setup, patching, backups, and monitoring.

**Other Cloud DB Services**: Similar managed features but would introduce multi-cloud complexity and additional learning curve.

### Decision

We chose Amazon RDS for PostgreSQL. It reduces operational burden by handling backups, updates, and availability, while integrating seamlessly with our AWS infrastructure.

### Status

Accepted — Amazon RDS is our database hosting platform for MVP and production.

### Consequences

**Positive:**

1. High reliability with managed backups and replication.

2. Simplifies maintenance, freeing the team to focus on development.

3. Seamless integration with AWS networking and security.

**Negative / Risks:**

1. Higher cost than self-managed EC2 instances.

**Future pivots:**

1. If costs become prohibitive, we could move to self-managed EC2 instances.
