# Security

This file defines the minimum security expectations for `[PROJECT_NAME]`.

## Reporting A Vulnerability

Report suspected vulnerabilities through `[SECURITY_REPORTING_CHANNEL]`.

Include:

- affected version or commit;
- summary of the issue;
- reproduction steps when safe to share;
- expected impact;
- relevant logs or screenshots with secrets removed.

Do not publicly disclose a vulnerability until the owner has reviewed it and approved disclosure.

## Supported Versions

| Version | Security Support |
| --- | --- |
| `[CURRENT_VERSION]` | `[SUPPORTED_OR_UNSUPPORTED]` |

Update this table when the project starts releasing versions.

## Secrets Policy

- Never commit secrets, credentials, tokens, private keys, or production configuration.
- Use placeholders in documentation and examples.
- Add `.env.example` only when the project has real environment variables to document.
- Rotate any secret that is accidentally committed.
- Treat AI prompts, logs, and generated artifacts as possible secret exposure surfaces.

## Sensitive Data And Credentials

Follow [.repository-mvp/project-start-guide.md](.repository-mvp/project-start-guide.md) before adapting this repository to a real project.

Use placeholders, fake examples, or role-based labels in committed files. Do not commit real personal names, personal emails, phone numbers, addresses, document IDs, customer data, production URLs, tokens, private keys, credentials, certificates, or secrets.

Store real credentials only in ignored local files such as `.env`, `.env.local`, `.secrets/`, or `.credentials/`. Commit `.env.example` only when it contains fake values or placeholders.

## Dependency And Supply Chain Guidance

This repository is stack-neutral today. After a stack is selected:

- document dependency ownership;
- enable dependency update automation where appropriate;
- review license and security implications before adding dependencies;
- pin versions when reproducibility matters;
- add dependency checks to CI/CD.

## AI Agent Security Rules

AI agents must:

- avoid exposing private data in prompts, logs, commits, issues, or pull requests;
- verify security-sensitive external claims from current primary sources;
- avoid adding authentication, authorization, encryption, or secret-handling behavior without explicit review;
- update security documentation when security posture changes.

## Security Readiness Checklist

- [ ] Security reporting channel is defined.
- [ ] Supported versions are defined once releases exist.
- [ ] Secrets handling is documented.
- [ ] Dependency review process is defined after stack selection.
- [ ] CI/CD includes security checks after the project has real code and dependencies.
