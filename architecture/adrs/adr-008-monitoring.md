## ADR 008: Monitoring & Logging — Amazon CloudWatch

### Context

Our application needs observability to track performance, errors, and resource usage. The monitoring solution should integrate easily with AWS infrastructure, provide alerting, and require minimal setup overhead for MVP.

### Options

**Amazon CloudWatch**: Native AWS monitoring service with metrics, logs, dashboards, and alarms. Integrates seamlessly with EC2 and RDS. Minimal setup required.

**Datadog**: Full-featured monitoring platform with APM, tracing, and custom dashboards. More powerful but higher cost and additional configuration effort.

**Sentry**: Focused on error tracking and application monitoring. Excellent for catching exceptions, stack traces, and user impact. Free tier only supports 1 user.

### Decision

We chose Amazon CloudWatch as our monitoring and logging solution. It integrates natively with our AWS infrastructure (EC2, RDS), offers reliable metrics and alarms, and requires minimal operational overhead—ideal for the MVP stage.

### Status

Accepted — CloudWatch will be our monitoring and logging tool for MVP and production.

### Consequences

**Positive:**

1. Seamless integration with AWS services (EC2, RDS, VPC).

2. Minimal setup and maintenance burden.

3. Provides dashboards, alarms, and log aggregation out-of-the-box.

**Negative / Risks:**

1. Less advanced application performance monitoring compared to Datadog.

2. Doesn’t capture application-level errors as effectively as Sentry.

**Future pivots:**

1. For error tracking and user impact visibility, we may integrate Sentry alongside CloudWatch.
