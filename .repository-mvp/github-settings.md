# GitHub Settings Guide

Use this guide after completing [project-start-guide.md](project-start-guide.md). These settings live in GitHub and cannot be fully enforced by repository files alone.

## Goal

Configure the repository so the default branch is protected, automation runs with least privilege, secrets are harder to leak, and future stack-specific security tools can be enabled intentionally.

## Critical Settings

### 1. Protect The Default Branch

Protect `main` with a repository ruleset or branch protection rule.

Recommended baseline:

- require a pull request before merging;
- require at least one approving review when collaboration begins;
- require status checks before merging;
- require branches to be up to date before merging when the project has active collaboration;
- block force pushes;
- block branch deletion;
- include administrators or repository owners when the project policy requires it.

Do not allow direct pushes to `main` after real project work begins.

### 2. Require Repository Hygiene Checks

Use the existing GitHub Actions workflow as the first required status check:

- `.github/workflows/repository-hygiene.yml`

After a stack is selected, add real checks for:

- formatting;
- linting;
- tests;
- API contract validation;
- security scanning;
- build verification.

### 3. Use Least-Privilege Access

Repository access should follow least privilege.

Recommended baseline:

- give write access only to maintainers who need it;
- use read access for observers;
- review administrator access regularly;
- prefer teams or roles over personal ownership in committed documentation;
- remove access when contributors leave the project.

### 4. Enable Security Features

Enable the security features available for the repository and organization plan.

Recommended baseline:

- dependency graph;
- Dependabot alerts;
- Dependabot security updates when a package ecosystem exists;
- secret scanning;
- push protection for secrets when available;
- private vulnerability reporting for public projects when appropriate.

Keep [.github/dependabot.yml](../.github/dependabot.yml) stack-neutral until a package ecosystem exists.

### 5. Configure Actions Safely

Recommended baseline:

- keep default workflow token permissions read-only unless a job needs write access;
- grant write permissions only at the job level and only for the minimum scope required;
- review third-party actions before use;
- prefer stable action versions;
- document stricter pinning policy in [../docs/quality.md](../docs/quality.md) if the project requires commit SHA pinning.

### 6. Enable Code Scanning After Stack Selection

Do not enable fake or empty code scanning.

Enable CodeQL, SAST, SCA, IaC scanning, SBOM generation, artifact signing, and provenance only after the project has enough stack context to configure them honestly.

Record the decision in:

- [../docs/architecture.md](../docs/architecture.md);
- [../docs/quality.md](../docs/quality.md);
- [../docs/compliance.md](../docs/compliance.md), when evidence is required.

## Setup Order

1. Complete [project-start-guide.md](project-start-guide.md).
2. Protect `main`.
3. Require repository hygiene checks.
4. Enable security features available to the repository.
5. Review access and ownership.
6. Add stack-specific checks only after stack selection.
7. Document evidence in [../docs/compliance.md](../docs/compliance.md) when compliance tracking is needed.

## Manual Review Checklist

- [ ] `main` is protected.
- [ ] Pull requests are required before merge.
- [ ] Required status checks are configured.
- [ ] Force pushes are blocked.
- [ ] Branch deletion is blocked.
- [ ] Repository access follows least privilege.
- [ ] Dependency graph is enabled when available.
- [ ] Dependabot alerts are enabled when available.
- [ ] Secret scanning and push protection are enabled when available.
- [ ] Code scanning is deferred until stack selection.
- [ ] GitHub Actions permissions are least-privilege by default.
