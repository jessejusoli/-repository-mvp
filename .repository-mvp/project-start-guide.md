# Project Start Guide

Use this guide before adapting this repository to any real project. Follow the steps in order, from most critical to least critical.

## Prime Rule

Never commit real sensitive data.

Use placeholders, fake examples, or role-based labels until the project has an approved way to handle real internal information.

Safe examples:

- `[PROJECT_NAME]`
- `[PROJECT_OWNER]`
- `[SECURITY_REPORTING_CHANNEL]`
- `user@example.com`
- `+1-555-0100`
- `https://example.com`
- `fake-token-for-docs-only`

Do not commit:

- real personal names;
- personal email addresses;
- phone numbers;
- home or office addresses;
- document IDs;
- customer data;
- production URLs;
- tokens;
- private keys;
- credentials;
- certificates;
- secrets;
- private logs;
- screenshots that expose real data.

## Step 1: Confirm The License

Start with [../LICENSE.md](../LICENSE.md).

Default position: proprietary and all rights reserved.

Before changing the license:

- confirm who owns the project;
- confirm whether the project can be public;
- confirm whether commercial use is allowed;
- confirm whether third-party assets or dependencies affect licensing;
- update [../README.md](../README.md) if the license changes.

Do not start implementation work before the project owner accepts the license posture.

## Step 2: Define Project Name And Purpose

Update [../README.md](../README.md) with placeholders or approved public-safe values:

- `[PROJECT_NAME]`
- `[PROJECT_PURPOSE]`
- `[CURRENT_VERSION]`
- `[OWNER]`
- `[PROJECT_STATUS]`
- `[PRIMARY_AUDIENCE]`

If the real project name is confidential, use a codename placeholder such as `[PROJECT_CODENAME]`.

The README is the front door. Keep it concise and link to deeper docs instead of duplicating policy.

## Step 3: Define Governance Without Real Personal Data

Update [../GOVERNANCE.md](../GOVERNANCE.md) using roles, teams, or placeholders.

Use:

- `[PROJECT_OWNER]`
- `[MAINTAINER]`
- `[SECURITY_OWNER]`
- `[RELEASE_OWNER]`
- `[OPERATIONS_OWNER]`
- `[APPROVER]`

Avoid real names, personal email addresses, phone numbers, or private team details unless the project owner explicitly approves publishing that information.

## Step 4: Configure Security And Support Channels Safely

Update [../SECURITY.md](../SECURITY.md) and [../SUPPORT.md](../SUPPORT.md) with safe placeholders first.

Use:

- `[SECURITY_REPORTING_CHANNEL]`
- `[GENERAL_SUPPORT_CHANNEL]`
- `[BUG_REPORT_CHANNEL]`
- `[INCIDENT_CHANNEL]`
- `[ESCALATION_OWNER]`

Do not put private phone numbers, personal emails, private Slack links, production dashboards, incident bridge URLs, or credential locations in committed files.

## Step 5: Protect Credentials Before Any Tooling Exists

Real credentials must live outside Git history.

Allowed local-only places:

- `.env`
- `.env.local`
- `.env.[LOCAL_NAME]`
- `.secrets/`
- `.credentials/`

Commit `.env.example` only when every value is fake or placeholder-based.

Good `.env.example` values:

```text
API_BASE_URL=https://example.com
API_TOKEN=fake-token-for-docs-only
DATABASE_URL=[LOCAL_DATABASE_URL]
```

Bad `.env.example` values:

```text
API_TOKEN=real-token
DATABASE_URL=real-production-url
PRIVATE_KEY=real-private-key
```

If a real secret is committed:

1. stop using it immediately;
2. rotate or revoke it;
3. remove it from current files;
4. review Git history exposure;
5. document the response path through [../SECURITY.md](../SECURITY.md);
6. add prevention checks before continuing.

## Step 6: Define The Current Vertical

Update [../VERTICAL.md](../VERTICAL.md).

Fill:

- Point A: current state;
- Point B: target state;
- version goal;
- success criteria;
- non-goals;
- decision boundaries.

Do not use the vertical as a roadmap or task list.

## Step 7: Review The Documentation System

Read [../docs/documentation-system.md](../docs/documentation-system.md) before adding more docs.

Use one source of truth:

- current version path: [../VERTICAL.md](../VERTICAL.md);
- future direction: [../ROADMAP.md](../ROADMAP.md);
- requirements: [../docs/requirements.md](../docs/requirements.md);
- candidate work: [../BACKLOG.md](../BACKLOG.md);
- active work: [../TASK_MANAGER.md](../TASK_MANAGER.md);
- completed changes: [../CHANGELOG.md](../CHANGELOG.md).

Add links, not duplicate explanations.

## Step 8: Define Requirements And Risks

Update:

- [../docs/requirements.md](../docs/requirements.md);
- [../docs/risk-register.md](../docs/risk-register.md);
- [../docs/glossary.md](../docs/glossary.md).

Keep requirements observable and avoid implementation details until a stack decision exists.

## Step 9: Plan Work

Use:

- [../BACKLOG.md](../BACKLOG.md) for candidate work;
- [../TASK_MANAGER.md](../TASK_MANAGER.md) for active work;
- [../CHANGELOG.md](../CHANGELOG.md) for completed notable changes.

Move only selected work from backlog into active tasks.

## Step 10: Configure Repository Collaboration

Update GitHub templates only with safe placeholders or approved public-safe values:

- [../.github/PULL_REQUEST_TEMPLATE.md](../.github/PULL_REQUEST_TEMPLATE.md);
- [../.github/ISSUE_TEMPLATE/bug_report.md](../.github/ISSUE_TEMPLATE/bug_report.md);
- [../.github/ISSUE_TEMPLATE/feature_request.md](../.github/ISSUE_TEMPLATE/feature_request.md);
- [../.github/CODEOWNERS](../.github/CODEOWNERS).

Keep real personal data out of templates.

## Step 11: Configure GitHub Repository Settings

Use [github-settings.md](github-settings.md) to configure settings that cannot be fully represented by repository files.

At minimum:

- protect `main`;
- require pull requests before merge;
- require repository hygiene checks;
- block force pushes;
- block branch deletion;
- enable dependency graph and Dependabot alerts when available;
- enable secret scanning and push protection when available;
- keep GitHub Actions permissions least-privilege.

## Step 12: Select Stack-Specific Tooling Last

Only after the previous steps are complete, decide whether to add:

- application source code;
- package manager files;
- framework configuration;
- database schemas;
- OpenAPI generation;
- CLI implementation;
- MCP server implementation;
- RAG server implementation;
- Docker Compose;
- Kubernetes;
- code scanning and dependency checks.

Document stack decisions in [../docs/architecture.md](../docs/architecture.md) before adding generated or tool-specific files.

Use [../docs/compliance.md](../docs/compliance.md) only as a readiness and evidence map. Do not claim compliance until the project owner has approved scope, evidence, legal review, and audit requirements.

## Final Safe-Start Checklist

- [ ] License is confirmed.
- [ ] Project name and purpose are safe to commit.
- [ ] Governance uses roles, teams, or placeholders.
- [ ] Security and support channels are placeholders or approved public-safe values.
- [ ] No real personal data is committed.
- [ ] No real credentials are committed.
- [ ] `.env.example` contains only fake values.
- [ ] Real credentials are stored only in ignored local files.
- [ ] `VERTICAL.md` defines the current version path.
- [ ] `docs/documentation-system.md` was reviewed before adding more docs.
- [ ] GitHub settings were reviewed with `.repository-mvp/github-settings.md`.
- [ ] Compliance readiness is tracked without claiming compliance.
- [ ] Stack-specific files are deferred until the stack is explicitly selected.
