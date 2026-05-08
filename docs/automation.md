# Automation Guidance

This project should evolve with automation as a first-class concern. Modern systems are consumed by humans, CI/CD pipelines, CLIs, AI agents, MCP servers, RAG systems, and deployment platforms.

## CI/CD

This MVP includes placeholders for multiple CI/CD platforms:

- GitHub Actions: `.github/workflows/repository-hygiene.yml`
- GitLab CI: `.gitlab-ci.yml`
- Azure Pipelines: `azure-pipelines.yml`

Each pipeline should eventually validate:

- repository hygiene;
- formatting and linting;
- tests;
- API contracts;
- security checks;
- build artifacts;
- deployment readiness.

## CLI

If the project needs command-line access, define a CLI that evolves with the system.

Minimum future documentation:

- command list;
- input and output contracts;
- exit codes;
- authentication behavior;
- examples for common workflows.

## MCP Server

If the project needs AI-agent integration, consider an MCP server that exposes safe project capabilities through documented tools and resources.

Minimum future documentation:

- supported tools;
- resource contracts;
- permissions model;
- audit logging;
- local and deployed usage.

## RAG Server

If the project needs retrieval-augmented generation, consider a RAG server that indexes approved project knowledge and evolves with the documentation.

Minimum future documentation:

- source documents;
- indexing cadence;
- chunking and metadata rules;
- freshness policy;
- access control;
- evaluation strategy.

## Docker Compose

If the project needs local multi-service orchestration, add Docker Compose after the stack is selected.

Minimum future documentation:

- service list;
- exposed ports;
- environment variables;
- volumes;
- startup order;
- health checks.

## Kubernetes

If the project needs orchestrated deployment, add Kubernetes manifests or Helm charts after deployment requirements are known.

Minimum future documentation:

- namespaces;
- workloads;
- services;
- ingress;
- config and secrets strategy;
- probes;
- resource requests and limits;
- rollout and rollback process.

## Automation Rule

Do not create automation that looks complete but cannot be trusted. Prefer a clear placeholder over a fake implementation.
