# Velora — Backend (Golang monorepo) TODO

## Repo setup
- [ ] Create monorepo root with README.md and LICENSE
- [ ] Add CODEOWNERS, CONTRIBUTING.md, .golangci.yml, .editorconfig
- [ ] Add .github/ISSUE_TEMPLATE and PR_TEMPLATE

## CI / Quality
- [ ] Add GitHub Actions: lint, vet, go test, sqlc generate, build, docker build+push
- [ ] Add Dependabot config
- [ ] Add gosec & staticcheck in pipeline

## Services (initial)
- [ ] auth-service
- [ ] agent-service
- [ ] workflow-service
- [ ] worker-service
- [ ] integration-service
- [ ] billing-service
- [ ] api-gateway
- [ ] shared libs (pkg/* and internal/*)

## Infra & local dev
- [ ] docker-compose for dev (Postgres, Redis, NATS, MinIO, Jaeger, Prometheus, Grafana)
- [ ] Makefile / quickstart script
- [ ] Helm chart (optional) / k8s manifests for core services

## Observability & Security
- [ ] OpenTelemetry integration skeleton
- [ ] Prometheus metrics handler & instrumentation
- [ ] Jaeger exporter
- [ ] Loki-compatible JSON logs via zap
- [ ] RBAC model + migration
- [ ] API key management + UI hooks

## DB & Migrations
- [ ] SQL schema + sqlc queries
- [ ] Flyway / golang-migrate migrations
- [ ] Postgres test container integration for integration tests

## LLM & Vector DB
- [ ] llm client interface + OpenAI-compatible adapter
- [ ] vector db adapter interface + local storage adapter

## Testing
- [ ] Unit tests for core packages
- [ ] Integration tests using testcontainers (Postgres)
- [ ] e2e example (run small workflow)

## Docs
- [ ] README per service + monorepo README
- [ ] API doc (OpenAPI yaml)
- [ ] Example workflow DSL docs & examples
