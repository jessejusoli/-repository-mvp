# Repository MVP Guidance

This directory contains adoption guidance for turning this universal repository starter into a real project repository.

It is intentionally separate from public project documentation. Public documentation belongs in `docs/`; adoption guidance belongs here.

## How To Use This Folder

1. Start with [project-start-guide.md](project-start-guide.md) before replacing any placeholders.
2. Use [github-settings.md](github-settings.md) to configure repository settings that cannot be committed as files.
3. Replace project placeholders in root files and `docs/`.
4. Define the current vertical goal in `VERTICAL.md`.
5. Select the project stack only when the project purpose requires it.
6. Add stack-specific files after the stack decision is documented.
7. Use [readme-guide.md](readme-guide.md) to improve the main README with badges, media, links, lists, citations, and GitHub repository signals.
8. Decide whether this guidance should remain tracked.

## Tracking Guidance

The root `.gitignore` includes a commented `.repository-mvp/` rule. Keep this folder tracked while adapting the template. After the project-specific structure is complete, uncomment the rule if this folder should become local-only guidance.

## Essential Adoption Order

1. `.repository-mvp/project-start-guide.md`
2. `.repository-mvp/github-settings.md`
3. `LICENSE.md`
4. `README.md`
5. `SECURITY.md`
6. `GOVERNANCE.md`
7. `SUPPORT.md`
8. `VERTICAL.md`
9. `AGENTS.md`
10. `CONTRIBUTING.md`
11. `docs/documentation-system.md`
12. `docs/README.md`
13. `docs/requirements.md`
14. `docs/compliance.md`
15. `BACKLOG.md`
16. `TASK_MANAGER.md`
17. `CHANGELOG.md`
18. CI/CD placeholders
19. README presentation improvements

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
