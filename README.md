# Vladimir Krauchuk

**Senior Golang Engineer · Distributed Systems · Cloud-Native Backend**

I am a backend engineer with 5+ years of commercial experience building
reliable services and event-driven systems. My primary focus is Go,
PostgreSQL, distributed workflows, performance, observability, and failure-safe
delivery.

## Core stack

- **Backend:** Go, REST, gRPC, microservices, event-driven architecture
- **Data and messaging:** PostgreSQL, Redis, Kafka, RabbitMQ, NATS
- **Infrastructure:** Docker, Kubernetes, AWS, CI/CD
- **Observability:** Prometheus, Grafana, OpenTelemetry, Jaeger
- **Engineering:** DDD, idempotency, concurrency, integration testing, profiling

## Featured projects

### [Solitaire Matchmaking](https://github.com/krav01/solitaire-matchmaking)

A production-oriented matchmaking and rating service for asynchronous
five-to-seven-player Solitaire tournaments.

- Balances room fill speed against immutable whole-room fairness constraints.
- Persists idempotent tournament transitions and outgoing events atomically.
- Uses bounded, lease-fenced workers for matching, deadlines, ordered rating,
  and at-least-once event delivery.
- Includes PostgreSQL lifecycle and resilience tests, race detection, fuzzing,
  vulnerability scanning, metrics, dashboards, and release documentation.

[Architecture](https://github.com/krav01/solitaire-matchmaking#architecture)
· [OpenAPI](https://github.com/krav01/solitaire-matchmaking/blob/main/api/openapi.yaml)
· [CI](https://github.com/krav01/solitaire-matchmaking/actions)

### [Usage Billing](https://github.com/krav01/usage-billing)

A Go and PostgreSQL service for metered API usage with frozen pricing and an
immutable processing ledger.

- Accepts retry-safe usage events and preserves their original unit price.
- Uses transactional work admission, concurrent `SKIP LOCKED` processing, and
  generation-fenced recovery.
- Covers crash recovery, integrity quarantine, exact integer accounting,
  monitoring, backup/restore, and reproducible performance evidence.

[Architecture](https://github.com/krav01/usage-billing/blob/main/docs/ARCHITECTURE.md)
· [Verification](https://github.com/krav01/usage-billing/blob/main/docs/VERIFICATION.md)
· [CI](https://github.com/krav01/usage-billing/actions)

### [Sunday System](https://github.com/krav01/homework)

A Go Kubernetes operator and persistent REST API built as a focused home
assignment.

- Recreates deleted Pods and applies template changes through serial rollouts.
- Preserves API data across Pod replacements with PVC-backed atomic storage.
- Verifies recovery through race tests, security checks, and live Docker/kind
  end-to-end scenarios with a replayable CI demonstration.

[Architecture](https://github.com/krav01/homework/blob/main/docs/ARCHITECTURE.md)
· [Demo](https://github.com/krav01/homework/blob/main/docs/DEMO.md)
· [CI](https://github.com/krav01/homework/actions)

### [Go CI Standards](https://github.com/krav01/go-ci-standards)

Reusable, least-privilege GitHub Actions workflows for Go repositories with
module, build, test, race, lint, and vulnerability gates.

## Engineering approach

I prefer explicit dependencies, small packages, stable contracts, and tests that
exercise retries, concurrency, partial failure, and recovery. Public projects
document their boundaries and evidence rather than hiding limitations behind a
"production-ready" label. Proprietary source code remains private.

[LinkedIn](https://www.linkedin.com/in/vladimir-krauchuk/)
