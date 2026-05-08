# Adoption Checklist

Use this checklist when converting the repository MVP into a project-specific repository.

## Safe Start

- [ ] Read `.repository-mvp/project-start-guide.md`.
- [ ] Review `.repository-mvp/github-settings.md` and configure GitHub settings manually.
- [ ] Confirm no real personal data will be committed.
- [ ] Confirm no real credentials, tokens, private keys, certificates, or production URLs will be committed.
- [ ] Confirm real credentials will live only in ignored local files such as `.env`, `.env.local`, `.secrets/`, or `.credentials/`.
- [ ] Confirm `.env.example` contains only fake values or placeholders.

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
- [ ] Use `docs/compliance.md` only as compliance readiness and evidence mapping, not as a compliance claim.
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
- [ ] Protect `main` with pull requests, required checks, and blocked force pushes.
- [ ] Enable dependency graph, Dependabot alerts, secret scanning, and push protection when available.
- [ ] Replace placeholder CI/CD commands with real project checks.
- [ ] Add stack-specific ignore rules after selecting the stack.
- [ ] Replace GitHub template placeholders when real repository ownership is known.
- [ ] Enable Dependabot ecosystems only after selecting a stack.
- [ ] Update `BACKLOG.md`, `TASK_MANAGER.md`, and `CHANGELOG.md`.

## Final Repository MVP Decision

- [ ] Decide whether `.repository-mvp/` remains tracked.
- [ ] If it should become local-only guidance, uncomment `.repository-mvp/` in `.gitignore`.
