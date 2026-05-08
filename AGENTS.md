# AI Agent Instructions

This file is the operating contract for AI agents, automation agents, and human reviewers using this repository.

## Prime Directive

Move the project toward the current vertical goal in [VERTICAL.md](VERTICAL.md). Do not expand horizontally into unrelated features, tools, frameworks, or documentation unless the current goal requires it.

## Required Behavior

- Work in en-US for all repository content unless a language-specific documentation folder already exists for the requested translation.
- Read [README.md](README.md), [VERTICAL.md](VERTICAL.md), [BACKLOG.md](BACKLOG.md), [TASK_MANAGER.md](TASK_MANAGER.md), and [CHANGELOG.md](CHANGELOG.md) before making project changes.
- Keep changes small, traceable, and aligned with the active task.
- Update living documentation in the same change that updates behavior, architecture, interfaces, or workflows.
- Preserve placeholders when the project has not made a decision yet.
- Prefer existing repository conventions over introducing new patterns.
- Do not select a runtime, framework, language, package manager, database, cloud provider, or deployment platform without an explicit project decision.

## Safety Rules

- Do not remove licensing, security, audit, or delivery documentation without replacing it with an approved alternative.
- Do not overwrite user work or unrelated changes.
- Do not generate large documentation sets when a concise linkable document is enough.
- Do not invent external facts, versions, pricing, laws, or vendor capabilities without verification from current primary sources.
- Do not commit secrets, credentials, private keys, tokens, or local environment files.

## Change Workflow

1. Confirm the requested work maps to the current vertical goal.
2. Identify the backlog item or task manager entry being addressed.
3. Make the smallest useful change.
4. Update affected documentation, backlog, task status, and changelog entries.
5. Run the relevant checks for the repository state.
6. Report what changed, what was verified, and what remains open.

## Documentation Expectations

- User-facing behavior belongs in [docs/README.md](docs/README.md).
- Architecture and major decisions belong in [docs/architecture.md](docs/architecture.md).
- API contract guidance belongs in [docs/api.md](docs/api.md).
- Automation, CI/CD, CLI, MCP, RAG, Docker, and Kubernetes guidance belongs in [docs/automation.md](docs/automation.md).

## Translation Policy

The source of truth is en-US. If a user needs another language, create a language-specific subdirectory such as `docs/pt-BR/` and keep the translated files clearly linked to their en-US source.
