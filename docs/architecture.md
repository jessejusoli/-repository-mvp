# Architecture And Decision Guidance

This project has not selected a technology stack yet. Use this document to record architectural direction as decisions become real.

## Architecture Snapshot

| Area | Current Decision |
| --- | --- |
| Runtime | `[RUNTIME_DECISION]` |
| Language | `[LANGUAGE_DECISION]` |
| Framework | `[FRAMEWORK_DECISION]` |
| Data storage | `[DATA_STORAGE_DECISION]` |
| API style | `[API_STYLE_DECISION]` |
| Deployment target | `[DEPLOYMENT_TARGET_DECISION]` |
| Observability | `[OBSERVABILITY_DECISION]` |

## Principles

- Document decisions before encoding them into tooling.
- Choose boring, maintainable technology unless the project goal requires otherwise.
- Keep humans, CI/CD systems, CLI users, AI agents, MCP clients, and RAG pipelines in mind when defining interfaces.
- Prefer explicit contracts over implicit behavior.

## Decision Record Template

Use this compact template for major decisions. Keep records in this file until the project needs a dedicated decision directory.

```md
## Decision: [DECISION_TITLE]

- Status: Proposed | Accepted | Superseded
- Date: [YYYY-MM-DD]
- Context: [WHY_THIS_DECISION_IS_NEEDED]
- Decision: [WHAT_WAS_DECIDED]
- Consequences: [EXPECTED_TRADEOFFS]
```

## Current Decisions

## Decision: Repository Starts Technology-Agnostic

- Status: Accepted
- Date: [YYYY-MM-DD]
- Context: The repository is intended to serve many possible projects.
- Decision: The MVP defines structure, documentation, and delivery expectations without selecting a runtime, framework, language, package manager, database, or cloud provider.
- Consequences: Future projects must make explicit stack decisions before adding generated files, runtime code, or deployment-specific configuration.
