# Repository MVP Guidance

This directory contains adoption guidance for turning this universal repository starter into a real project repository.

It is intentionally separate from public project documentation. Public documentation belongs in `docs/`; adoption guidance belongs here.

## How To Use This Folder

1. Start with [project-start-guide.md](project-start-guide.md) before replacing any placeholders.
2. Replace project placeholders in root files and `docs/`.
3. Define the current vertical goal in `VERTICAL.md`.
4. Select the project stack only when the project purpose requires it.
5. Add stack-specific files after the stack decision is documented.
6. Use [readme-guide.md](readme-guide.md) to improve the main README with badges, media, links, lists, citations, and GitHub repository signals.
7. Decide whether this guidance should remain tracked.

## Tracking Guidance

The root `.gitignore` includes a commented `.repository-mvp/` rule. Keep this folder tracked while adapting the template. After the project-specific structure is complete, uncomment the rule if this folder should become local-only guidance.

## Essential Adoption Order

1. `.repository-mvp/project-start-guide.md`
2. `LICENSE.md`
3. `README.md`
4. `SECURITY.md`
5. `GOVERNANCE.md`
6. `SUPPORT.md`
7. `VERTICAL.md`
8. `AGENTS.md`
9. `CONTRIBUTING.md`
10. `docs/documentation-system.md`
11. `docs/README.md`
12. `docs/requirements.md`
13. `BACKLOG.md`
14. `TASK_MANAGER.md`
15. `CHANGELOG.md`
16. CI/CD placeholders
17. README presentation improvements

## Do Not Add Yet

Do not add these until the project makes explicit decisions:

- application source code;
- package manager lockfiles;
- framework configuration;
- database schemas;
- generated API clients;
- real deployment manifests;
- secrets or environment-specific configuration.
- real personal data, credentials, tokens, private keys, or production URLs.
