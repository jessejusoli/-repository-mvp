# [PROJECT_NAME]

[![Template](https://img.shields.io/badge/template-universal-blue)](.repository-mvp/README.md)
[![Documentation](https://img.shields.io/badge/docs-living-brightgreen)](docs/README.md)
[![AI Agents](https://img.shields.io/badge/agents-ready-purple)](AGENTS.md)
[![License](https://img.shields.io/badge/license-proprietary-lightgrey)](LICENSE.md)

[PROJECT_PURPOSE]

This repository is a universal project starter for building software with clear structure, living documentation, AI-agent guidance, and disciplined delivery practices. Replace every placeholder before using it as the source of truth for a real project.

## Project Snapshot

| Field | Value |
| --- | --- |
| Project | `[PROJECT_NAME]` |
| Purpose | `[PROJECT_PURPOSE]` |
| Current version | `[CURRENT_VERSION]` |
| Owner | `[OWNER]` |
| Status | `[PROJECT_STATUS]` |
| Primary audience | `[PRIMARY_AUDIENCE]` |

## Start Here

1. Read [VERTICAL.md](VERTICAL.md) to understand the current version goal from Point A to Point B.
2. Read [AGENTS.md](AGENTS.md) before using any AI agent or automation workflow in this repository.
3. Replace placeholders in this README and the living documentation under [docs/](docs/README.md).
4. Use [BACKLOG.md](BACKLOG.md), [TASK_MANAGER.md](TASK_MANAGER.md), and [CHANGELOG.md](CHANGELOG.md) to plan, execute, and record changes.
5. Review [.repository-mvp/](.repository-mvp/README.md) while adapting this template, then decide whether to keep tracking it.

## Documentation

- [Project documentation and user guide](docs/README.md)
- [Architecture and decision guidance](docs/architecture.md)
- [API documentation guidance](docs/api.md)
- [Automation guidance](docs/automation.md)

Documentation must stay alive with the project. Update the related document in the same change that modifies behavior, architecture, API contracts, operations, or user workflows.

## Repository Principles

- Keep the repository technology-agnostic until the project explicitly selects a stack.
- Prefer clear contracts, documented decisions, and small reversible changes.
- Treat humans, AI agents, CI/CD systems, CLIs, MCP servers, and RAG servers as first-class project consumers.
- Keep the default language en-US. Add translations only under language-specific folders such as `docs/pt-BR/`.
- Do not add stack-specific generated files until the project has chosen that stack.

## Delivery System

This MVP includes guidance and placeholders for:

- CI/CD across GitHub Actions, GitLab CI, and Azure Pipelines.
- API documentation with OpenAPI and viewers such as Swagger UI, Scalar, and Redoc.
- Future CLI, MCP server, and RAG server capabilities.
- Future Docker Compose and Kubernetes deployment definitions.

The placeholder files intentionally avoid choosing a runtime, package manager, container image, database, cloud provider, or application framework.

## License

This project starts as proprietary by default. See [LICENSE.md](LICENSE.md). Replace it only after the owner intentionally selects another license.
