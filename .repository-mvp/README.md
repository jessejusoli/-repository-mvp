# Repository MVP Guidance

This directory contains adoption guidance for turning this universal repository starter into a real project repository.

It is intentionally separate from public project documentation. Public documentation belongs in `docs/`; adoption guidance belongs here.

## How To Use This Folder

1. Replace project placeholders in root files and `docs/`.
2. Define the current vertical goal in `VERTICAL.md`.
3. Select the project stack only when the project purpose requires it.
4. Add stack-specific files after the stack decision is documented.
5. Decide whether this guidance should remain tracked.

## Tracking Guidance

The root `.gitignore` includes a commented `.repository-mvp/` rule. Keep this folder tracked while adapting the template. After the project-specific structure is complete, uncomment the rule if this folder should become local-only guidance.

## Essential Adoption Order

1. `README.md`
2. `LICENSE.md`
3. `VERTICAL.md`
4. `AGENTS.md`
5. `docs/README.md`
6. `BACKLOG.md`
7. `TASK_MANAGER.md`
8. `CHANGELOG.md`
9. CI/CD placeholders

## Do Not Add Yet

Do not add these until the project makes explicit decisions:

- application source code;
- package manager lockfiles;
- framework configuration;
- database schemas;
- generated API clients;
- real deployment manifests;
- secrets or environment-specific configuration.
