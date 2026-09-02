# Vladimir Krauchuk

**Senior Backend Engineer · Go**

I build backend services in Go, focusing on clear API contracts, event-driven
systems, and reliable infrastructure. I care about what happens when requests
are retried, dependencies fail, or a service needs to recover.

## Core stack

- **Backend:** Go, REST APIs, gRPC, microservices
- **Data and messaging:** PostgreSQL, Redis, Kafka
- **Infrastructure:** Docker, Kubernetes, AWS, CI/CD
- **Observability:** Prometheus, Grafana, OpenTelemetry, Jaeger
- **Quality:** unit and integration tests, race detection, profiling, code review

## Featured project

### [Sunday System](https://github.com/krav01/homework)

A Go and Kubernetes home assignment with an `EtherealPod` custom controller and
a persistent groceries API.

- Recreates deleted Pods and applies template changes through serial rollouts.
- Preserves grocery data on a PVC, with an exclusive writer lock and explicit
  handling of storage failures.
- Includes race tests, linting, vulnerability checks, and live Docker/kind
  acceptance tests.
- Documents the design tradeoffs, recovery behavior, and limits of the solution.

[Architecture](https://github.com/krav01/homework/blob/main/docs/ARCHITECTURE.md)
· [Demo walkthrough](https://github.com/krav01/homework/blob/main/docs/DEMO.md)
· [Checks](https://github.com/krav01/homework/actions)

## How I approach engineering

I prefer explicit dependencies, small packages, and tests that exercise failure
paths. I document the limits of a design instead of hiding them behind a
"production-ready" label. My public projects are independent work; proprietary
source code stays private.

[LinkedIn](https://www.linkedin.com/in/vladimir-krauchuk/)
