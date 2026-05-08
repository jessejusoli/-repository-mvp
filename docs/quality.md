# Quality

This file defines how `[PROJECT_NAME]` verifies quality. It does not define feature scope or active tasks.

## Quality Goals

| Area | Standard | Current Status |
| --- | --- | --- |
| Correctness | `[CORRECTNESS_STANDARD]` | Proposed |
| Maintainability | `[MAINTAINABILITY_STANDARD]` | Proposed |
| Security | See [../SECURITY.md](../SECURITY.md). | Proposed |
| Documentation | Living docs updated with behavior changes. | Active |
| Accessibility | `[ACCESSIBILITY_STANDARD]` | Proposed |
| Performance | `[PERFORMANCE_STANDARD]` | Proposed |

## Testing Strategy

Define the project testing layers after the stack is selected.

| Layer | Purpose | Required When |
| --- | --- | --- |
| Unit tests | Validate isolated logic. | The project has testable code units. |
| Integration tests | Validate module or service collaboration. | The project has multiple integrated parts. |
| Contract tests | Validate API, CLI, MCP, or event contracts. | The project exposes stable interfaces. |
| End-to-end tests | Validate critical user workflows. | The project has user-facing workflows. |
| Security checks | Validate known security risks. | The project has dependencies, auth, data, or deployment. |

## Review Checklist

- [ ] The change supports [../VERTICAL.md](../VERTICAL.md).
- [ ] The right source-of-truth document was updated.
- [ ] Requirements and acceptance criteria are clear when behavior changes.
- [ ] Tests or verification steps match the risk of the change.
- [ ] No secrets, private data, or misleading placeholders were introduced.
- [ ] The changelog was updated when needed.

## Quality Gates

Before release, the project should define:

- required checks;
- minimum review approvals;
- security review triggers;
- documentation review triggers;
- compatibility expectations;
- rollback requirements.

## Current MVP Gate

The repository starter is acceptable when required files exist, local links work, YAML placeholders parse, and no stack-specific runtime has been introduced.
