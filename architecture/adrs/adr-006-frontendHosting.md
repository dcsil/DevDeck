## ADR 006: Frontend Hosting — Vercel

### Context

We need a hosting platform for our React frontend that supports fast deployment, global availability, and preview environments for rapid iteration. The platform should integrate smoothly with our GitHub workflow.

### Options

**Vercel**: Optimized for React and Next.js, automatic deployments from GitHub, built-in SSL, and preview environments, with a generous free tier.

**Netlify**: Similar features (CDN, SSL, GitHub integration)

**Custom Hosting on AWS S3 + CloudFront**: Highly flexible and cost-efficient, but requires manual setup of deployment pipelines

### Decision

We chose Vercel to host our React frontend. It has a generous free tier and integrates seamlessly with our GitHub workflow.

### Status

Accepted — Vercel will be our primary hosting platform for the frontend during MVP and initial production.

### Consequences

**Positive:**

1. Minimal setup and immediate CI/CD integration with GitHub.

2. Global CDN ensures fast performance for users worldwide.

3. Preview deployments simplify collaboration and user testing.

**Negative / Risks:**

1. Less flexibility than custom hosting (limited to Vercel’s platform constraints).

**Future pivots:**

1. If costs or platform limitations arise, we may migrate to Netlify or a custom AWS S3 + CloudFront setup.
