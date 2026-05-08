# Operations

This file defines operational readiness for `[PROJECT_NAME]`.

## Current Status

No deployable or operable system exists yet. Keep this file as a placeholder until the project selects a stack and creates something that runs.

## Operations Boundaries

- Automation strategy belongs in [automation.md](automation.md).
- Architecture decisions belong in [architecture.md](architecture.md).
- Release process belongs in [release.md](release.md).
- Runtime operating procedures belong here once runtime exists.

## Future Operational Readiness

When the project has a runtime, define:

- environments;
- deployment process;
- configuration and secrets handling;
- monitoring and alerting;
- logs and traces;
- backup and restore;
- incident response;
- capacity and scaling;
- runbooks;
- service-level expectations.

## Runbook Template

```md
## Runbook: [RUNBOOK_NAME]

- Trigger: [WHEN_TO_USE_THIS_RUNBOOK]
- Impact: [USER_OR_SYSTEM_IMPACT]
- Owner: [OWNER]
- Steps:
  1. [STEP]
  2. [STEP]
- Verification: [HOW_TO_CONFIRM_RECOVERY]
- Escalation: [WHO_TO_CONTACT]
```

## Activation Rule

Activate this document when the project introduces a local service, deployed service, scheduled job, data store, or operational dependency.
