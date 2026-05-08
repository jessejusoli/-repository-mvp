# Governance

This file defines how decisions are made for `[PROJECT_NAME]`.

## Governance Principles

- Decisions should be explicit, documented, and reversible when possible.
- The current vertical goal in [VERTICAL.md](VERTICAL.md) controls near-term scope.
- Architecture decisions belong in [docs/architecture.md](docs/architecture.md).
- Project direction beyond the current vertical belongs in [ROADMAP.md](ROADMAP.md).
- Active execution belongs in [TASK_MANAGER.md](TASK_MANAGER.md).

## Roles

| Role | Owner | Responsibilities |
| --- | --- | --- |
| Project owner | `[PROJECT_OWNER]` | Final accountability for purpose, scope, and license. |
| Maintainer | `[MAINTAINER]` | Reviews changes, keeps docs current, protects repository quality. |
| Security owner | `[SECURITY_OWNER]` | Handles vulnerabilities and security process. |
| Release owner | `[RELEASE_OWNER]` | Coordinates versioning, release readiness, and rollback decisions. |
| Operations owner | `[OPERATIONS_OWNER]` | Owns runtime operations once something deployable exists. |

## Decision Rights

| Decision Type | Source Of Truth | Approval |
| --- | --- | --- |
| Project purpose and scope | `README.md`, `VERTICAL.md` | `[APPROVER]` |
| License changes | `LICENSE.md` | `[APPROVER]` |
| Architecture decisions | `docs/architecture.md` | `[APPROVER]` |
| Security posture | `SECURITY.md` | `[APPROVER]` |
| Release process | `docs/release.md` | `[APPROVER]` |
| Operational readiness | `docs/operations.md` | `[APPROVER]` |

## Approval Rules

- Changes that alter project purpose, license, security posture, architecture, release policy, or operational behavior require owner review.
- Routine documentation and task updates may be approved by maintainers.
- AI-generated changes require the same review standard as human-written changes.

## Conflict Resolution

When contributors disagree:

1. restate the decision being made;
2. identify the source-of-truth document;
3. compare options against the current vertical goal;
4. document the final decision and consequences;
5. update related files to prevent future ambiguity.

## Maintenance Cadence

Review governance after major releases, ownership changes, security events, or changes to the project audience.
