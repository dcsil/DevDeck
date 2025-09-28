## ADR 003: Database Technology — PostgreSQL

### Context

Our application needs a database to handle structured data with strong consistency, transactional support, and the flexibility to evolve with our product.

### Options

**PostgreSQL**: Open-source relational database, advanced features (JSONB), widely supported on cloud providers.

**MySQL**: Popular relational database, simpler and performant for common queries, but less feature-rich than PostgreSQL for semi-structured data.

**NoSQL (e.g., MongoDB)**: Flexible schema-less design, scales horizontally, but weaker transactional guarantees and less suited for relational queries.

### Decision

We chose PostgreSQL as our database. It offers the best balance between relational integrity, advanced features, and ecosystem support. Its JSONB capabilities give us some flexibility for semi-structured data while keeping strong ACID compliance.

### Status

Accepted — PostgreSQL will serve as the core database for MVP and production.

### Consequences

**Positive:**

1. Reliable relational model

2. Flexible enough for semi-structured data.

3. Mature ecosystem and strong tooling support.

**Negative / Risks:**

1. Requires schema management and migrations.

**Future pivots:**

1. If workloads become predominantly unstructured, we may supplement with a NoSQL store.

2. If our scale demands specialized analytics, we may integrate a columnar data warehouse.
