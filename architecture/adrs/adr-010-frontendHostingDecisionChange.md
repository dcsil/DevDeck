# ADR 010: Frontend Deployment — GitHub Actions → Vercel (Private Repo)

## Status
**Accepted** — **Supersedes ADR 006** (Frontend Hosting — Vercel)

## Context
We originally selected Vercel with Git-based auto-deploys (ADR 006). For a **private** GitHub repository, Vercel’s native auto-deploy requires a **paid Pro plan**. We want to keep the repo private and avoid new hosting costs.

## Options
- **A. Vercel Git Integration (Private Repo)** — Requires Pro plan for seamless auto-deploys.
- **B. GitHub Actions → Vercel CLI (Private Repo)** — Keep repo private; deploy via Vercel token in CI.
- **C. Netlify (Private Repo)** — Similar constraints; paid features for some private-repo workflows.
- **D. AWS S3 + CloudFront** — Flexible/low cost but more DevOps work; weaker built-in preview flow.

## Decision
Adopt **GitHub Actions–based CD** that builds the React app and **deploys to Vercel via CLI** using a token stored in GitHub Secrets. This preserves privacy, keeps Vercel’s global CDN, and avoids Vercel Pro fees for now.

## Consequences

### Positive
1. Repository remains **private** without paying for Pro.
2. Retain Vercel’s **global CDN** and preview deployments on the **Hobby** tier.
3. Unified CI/CD in **GitHub Actions** (consistent with backend pipeline).

### Negative / Risks
1. We own **pipeline maintenance** (YAML, tokens, caching).
2. Some native Vercel features (e.g., automatic per-PR previews) need **custom CI wiring**.
3. **Secret management** and token rotation required.