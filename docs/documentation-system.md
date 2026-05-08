# Documentation System

This file explains where information belongs so the repository does not grow duplicate sources of truth.

## Core Rule

Every important fact should have one primary home. Other files may summarize and link to that home, but they should not duplicate the full content.

## Source-Of-Truth Map

| Information Type | Primary Home |
| --- | --- |
| Template adoption order and safe-start workflow | [../.repository-mvp/project-start-guide.md](../.repository-mvp/project-start-guide.md) |
| GitHub repository settings guidance | [../.repository-mvp/github-settings.md](../.repository-mvp/github-settings.md) |
| Project front door and quick navigation | [../README.md](../README.md) |
| Current version Point A to Point B | [../VERTICAL.md](../VERTICAL.md) |
| Future direction and milestones | [../ROADMAP.md](../ROADMAP.md) |
| Candidate work | [../BACKLOG.md](../BACKLOG.md) |
| Active execution | [../TASK_MANAGER.md](../TASK_MANAGER.md) |
| Completed notable changes | [../CHANGELOG.md](../CHANGELOG.md) |
| Contribution workflow | [../CONTRIBUTING.md](../CONTRIBUTING.md) |
| Security policy | [../SECURITY.md](../SECURITY.md) |
| Support routing | [../SUPPORT.md](../SUPPORT.md) |
| Governance and decision rights | [../GOVERNANCE.md](../GOVERNANCE.md) |
| Professional conduct | [../CODE_OF_CONDUCT.md](../CODE_OF_CONDUCT.md) |
| Architecture decisions | [architecture.md](architecture.md) |
| Requirements and acceptance criteria | [requirements.md](requirements.md) |
| Compliance readiness and evidence mapping | [compliance.md](compliance.md) |
| API documentation strategy | [api.md](api.md) |
| Automation strategy | [automation.md](automation.md) |
| Quality strategy | [quality.md](quality.md) |
| Release process | [release.md](release.md) |
| Operations readiness | [operations.md](operations.md) |
| Canonical terms | [glossary.md](glossary.md) |
| Known risks | [risk-register.md](risk-register.md) |

## Anti-Duplication Rules

- `README.md` summarizes and links; it does not store deep policy.
- `.repository-mvp/project-start-guide.md` defines template adoption order; it does not replace project security policy.
- `.repository-mvp/github-settings.md` guides manual GitHub settings; it does not replace committed policy files.
- `docs/compliance.md` maps readiness and evidence; it does not claim compliance or replace legal review.
- `VERTICAL.md` defines the current version path; it does not hold roadmap or task lists.
- `ROADMAP.md` describes future direction; it does not track active work.
- `BACKLOG.md` lists candidate work; it does not replace requirements.
- `TASK_MANAGER.md` tracks active work; it does not define strategy.
- `CHANGELOG.md` records completed changes; it does not plan future work.
- `GOVERNANCE.md` defines decision rights; it does not document technical design.
- `docs/architecture.md` records technical decisions; it does not assign governance ownership.
- `docs/requirements.md` defines what must be true; it does not define implementation steps.
- `docs/quality.md` defines verification expectations; it does not hold feature scope.
- `docs/release.md` defines release process; it does not duplicate changelog entries.
- `docs/operations.md` defines runtime operations only after something operable exists.

## Update Workflow

1. Identify the primary home for the information.
2. Update that file.
3. Add short links from related files only when navigation helps.
4. Remove duplicate explanations that would drift over time.
5. Update [../CHANGELOG.md](../CHANGELOG.md) when the documentation change affects repository structure, policy, or user-facing behavior.
