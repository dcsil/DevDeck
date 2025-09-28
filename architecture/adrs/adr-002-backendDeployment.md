## ADR 002: Backend Deployment Environment — AWS EC2

### Context

We need a reliable and cost-effective way to deploy our backend service and ensure it can communicate with the database, external APIs (e.g., OpenAI), and monitoring tools. The deployment environment should support Dockerized applications and provide flexibility for scaling as the project evolves. Our goal is to start with minimal overhead for MVP deployment while maintaining clear paths to scale later.

### Options

**AWS EC2**: Virtual machines with full control over OS and networking. Supports Docker easily. Requires manual setup for scaling and patching.

**AWS Lambda + API Gateway**: Fully serverless, pay-per-request. Great for spiky workloads, but limited for long-lived connections and complex deployment pipelines.

**Render**: Developer-friendly, abstracted infra. Fast to set up but limited control, may not meet enterprise deployment requirements.

**GCP**: Similar offerings but require an additional learning curve.

### Decision

We chose to deploy our backend on AWS EC2 instances. This gives us direct control over the runtime, networking, and scaling strategy while keeping initial complexity low.

### Status

Accepted — this is our deployment strategy for MVP and early production.

### Consequences

**Positive:**

1. Simplicity: low setup cost compared to ECS or Kubernetes.

2. Flexibility: full control over OS, Docker runtime, and networking.

3. Cost-effective because AWS has a generous free tier.

**Negative / Risks:**

1. Scaling requires manual configuration, such as using auto-scaling groups.

2. Less “managed” than serverless options like Lambda.

**Future pivots:**

1. If workload patterns are bursty and event-driven, parts of the system can move to Lambda + API Gateway.
