# Contributing

This file defines how humans and AI agents contribute to `[PROJECT_NAME]`.

## Contribution Principles

- Keep every change aligned with [VERTICAL.md](VERTICAL.md).
- Use [BACKLOG.md](BACKLOG.md) for candidate work and [TASK_MANAGER.md](TASK_MANAGER.md) for active work.
- Update living documentation in the same change that updates behavior, architecture, interfaces, operations, or project workflow.
- Do not add stack-specific tooling until the stack decision is recorded in [docs/architecture.md](docs/architecture.md).
- Keep changes small enough to review with confidence.

## Branch Naming

Use clear, traceable branch names:

- `feature/[short-outcome]`
- `fix/[short-problem]`
- `docs/[short-topic]`
- `chore/[short-maintenance-task]`

Examples:

- `docs/add-quality-guidance`
- `chore/update-repository-hygiene`

## Commit Guidance

Use concise commit messages that explain the outcome:

```text
docs: add repository quality guidance
chore: add universal git attributes
```

Prefer one logical change per commit. Avoid mixing unrelated documentation, policy, and implementation changes.

## Pull Request Expectations

Every pull request should include:

- the problem or outcome;
- the related backlog item or task when one exists;
- the changed documentation;
- the checks that were run;
- remaining risks or follow-up work.

Use [.github/PULL_REQUEST_TEMPLATE.md](.github/PULL_REQUEST_TEMPLATE.md) when working on GitHub.

## Review Rules

Reviewers should verify:

- the change supports the current vertical goal;
- the correct source-of-truth document was updated;
- no duplicate planning or policy content was introduced;
- no secrets or private environment details were committed;
- checks are appropriate for the current project maturity.

## Definition Of Done

A change is done when:

- the expected outcome is complete;
- relevant docs are updated;
- checks pass or blocked checks are explained;
- [CHANGELOG.md](CHANGELOG.md) is updated for user-visible, structural, or policy changes;
- active tasks are updated in [TASK_MANAGER.md](TASK_MANAGER.md).

## Where Information Belongs

When unsure where to document something, use [docs/documentation-system.md](docs/documentation-system.md). Do not duplicate the same policy or plan in multiple files.
