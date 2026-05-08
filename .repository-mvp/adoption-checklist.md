# Adoption Checklist

Use this checklist when converting the repository MVP into a project-specific repository.

## Identity

- [ ] Replace `[PROJECT_NAME]`.
- [ ] Replace `[PROJECT_PURPOSE]`.
- [ ] Replace `[OWNER]`.
- [ ] Confirm the default proprietary license or replace it intentionally.

## Direction

- [ ] Fill Point A in `VERTICAL.md`.
- [ ] Fill Point B in `VERTICAL.md`.
- [ ] Define success criteria.
- [ ] Define non-goals.

## Documentation

- [ ] Update the README start-here flow.
- [ ] Update the user guide in `docs/README.md`.
- [ ] Record initial architecture decisions in `docs/architecture.md`.
- [ ] Define API documentation expectations in `docs/api.md`.
- [ ] Define automation expectations in `docs/automation.md`.

## Delivery

- [ ] Choose CI/CD platform ownership.
- [ ] Replace placeholder CI/CD commands with real project checks.
- [ ] Add stack-specific ignore rules after selecting the stack.
- [ ] Update `BACKLOG.md`, `TASK_MANAGER.md`, and `CHANGELOG.md`.

## Final Repository MVP Decision

- [ ] Decide whether `.repository-mvp/` remains tracked.
- [ ] If it should become local-only guidance, uncomment `.repository-mvp/` in `.gitignore`.
