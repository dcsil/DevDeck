## ADR 007: LLM Integration — OpenAI API

### Context

Our application requires LLM to generate content. We need an integration that is reliable, accurate, and fast to implement for our MVP. The solution should minimize hallucinations in outputs, deliver responses with low latency, and remain cost-effective as usage grows.

### Options

**OpenAI API**: State-of-the-art models accessible via simple REST API. Offers high accuracy, low latency, and competitive pricing. No infrastructure to manage.

**Self-hosted Models (e.g., Hugging Face + custom inference)**: Full control, avoids vendor dependency, but requires GPUs, DevOps resources, and ML expertise. Higher upfront and scaling costs.

**Alternative AI Providers (e.g., Anthropic, Cohere)**: Similar API-based offerings. Some models excel at safety, but ecosystems are smaller and may be less optimized for latency or cost compared to OpenAI.

### Decision

We chose the OpenAI API to provide AI functionality. It has demonstrated the lowest hallucination rates, offers low latency, and is cost-effective relative to alternatives. It enables us to deliver features quickly without the need to manage infrastructure or ML models ourselves.

### Status

Accepted — OpenAI API will be our initial AI provider for MVP and production.

### Consequences

**Positive:**

1. Best-in-class model accuracy with fewer hallucinations.

2. Low-latency responses, supporting smooth user experience.

3. Competitive pricing makes it affordable for MVP and early scaling.

4. Rapid integration with minimal development effort.

**Negative / Risks:**

1. Latency and uptime tied to an external service.

**Future pivots:**

1. If costs, availability, or vendor lock-in become problematic, we may explore adding a fallback provider (Anthropic, Cohere) or running a self-hosted model on GPUs.
