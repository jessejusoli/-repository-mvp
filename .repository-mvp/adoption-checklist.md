# Adoption Checklist

Use this checklist when converting the repository MVP into a project-specific repository.

## Identity

- [ ] Replace `[PROJECT_NAME]`.
- [ ] Replace `[PROJECT_PURPOSE]`.
- [ ] Replace `[OWNER]`.
- [ ] Confirm the default proprietary license or replace it intentionally.
- [ ] Define project owner, maintainers, security owner, release owner, and operations owner in `GOVERNANCE.md`.
- [ ] Define support, security, conduct, and escalation channels.

## Direction

- [ ] Fill Point A in `VERTICAL.md`.
- [ ] Fill Point B in `VERTICAL.md`.
- [ ] Define success criteria.
- [ ] Define non-goals.
- [ ] Use `ROADMAP.md` only for future direction beyond the current vertical.

## Documentation

- [ ] Update the README start-here flow.
- [ ] Improve the README with useful badges, images, videos, links, lists, citations, and GitHub repository links where they help the reader.
- [ ] Review `docs/documentation-system.md` and confirm each source-of-truth boundary.
- [ ] Update the user guide in `docs/README.md`.
- [ ] Define initial requirements in `docs/requirements.md`.
- [ ] Record initial architecture decisions in `docs/architecture.md`.
- [ ] Define API documentation expectations in `docs/api.md`.
- [ ] Define automation expectations in `docs/automation.md`.
- [ ] Define quality expectations in `docs/quality.md`.
- [ ] Define release expectations in `docs/release.md`.
- [ ] Keep `docs/operations.md` inactive until something operable exists.
- [ ] Add domain terms to `docs/glossary.md`.
- [ ] Add known risks to `docs/risk-register.md`.

## Delivery

- [ ] Choose CI/CD platform ownership.
- [ ] Replace placeholder CI/CD commands with real project checks.
- [ ] Add stack-specific ignore rules after selecting the stack.
- [ ] Replace GitHub template placeholders when real repository ownership is known.
- [ ] Enable Dependabot ecosystems only after selecting a stack.
- [ ] Update `BACKLOG.md`, `TASK_MANAGER.md`, and `CHANGELOG.md`.

## Final Repository MVP Decision

- [ ] Decide whether `.repository-mvp/` remains tracked.
- [ ] If it should become local-only guidance, uncomment `.repository-mvp/` in `.gitignore`.
