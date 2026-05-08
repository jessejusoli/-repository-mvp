# Compliance Readiness

This file tracks compliance readiness for `[PROJECT_NAME]`.

## No Compliance Claim

This repository does not claim compliance with any framework, law, regulation, certification, or standard.

Use this file only as a readiness and evidence map. Real compliance depends on project scope, organization policy, legal review, data type, runtime behavior, operations, vendors, jurisdiction, and audit requirements.

## Source-Of-Truth Boundaries

- Security policy belongs in [../SECURITY.md](../SECURITY.md).
- Governance and decision rights belong in [../GOVERNANCE.md](../GOVERNANCE.md).
- Requirements belong in [requirements.md](requirements.md).
- Quality checks belong in [quality.md](quality.md).
- Release process belongs in [release.md](release.md).
- Operations evidence belongs in [operations.md](operations.md) once something operable exists.
- GitHub repository settings guidance belongs in [../.repository-mvp/github-settings.md](../.repository-mvp/github-settings.md).

## Compliance Context

| Field | Value |
| --- | --- |
| Framework | `[COMPLIANCE_FRAMEWORK]` |
| Scope | `[COMPLIANCE_SCOPE]` |
| Data types | `[DATA_TYPES]` |
| Jurisdiction | `[JURISDICTION]` |
| Owner | `[COMPLIANCE_OWNER]` |
| Review cadence | `[REVIEW_CADENCE]` |
| Status | Proposed |

## Control Readiness Matrix

| Control ID | Framework Reference | Control Intent | Evidence Location | Owner | Status | Risk |
| --- | --- | --- | --- | --- | --- | --- |
| `CTRL-001` | `[COMPLIANCE_FRAMEWORK_REFERENCE]` | `[CONTROL_INTENT]` | `[EVIDENCE_LOCATION]` | `[OWNER]` | Proposed | `[RISK]` |

## Evidence Rules

- Do not store secrets, private data, credentials, customer data, or production evidence in this repository.
- Use placeholders for evidence that cannot be safely committed.
- Link to approved evidence locations only when those links are safe to expose.
- Keep evidence current with the review cadence.
- Do not mark a control as satisfied without owner review.

## Automation Readiness

Enable compliance-related automation only after the project has selected a stack and risk profile.

Future automation may include:

- CodeQL or another SAST tool;
- software composition analysis;
- secret scanning;
- infrastructure-as-code scanning;
- SBOM generation;
- artifact signing;
- provenance or attestation generation;
- policy-as-code checks.

## Review Checklist

- [ ] Compliance scope is defined.
- [ ] Compliance owner is defined.
- [ ] Data types are documented.
- [ ] Jurisdiction is documented.
- [ ] Controls are mapped to evidence.
- [ ] Evidence locations are safe to reference.
- [ ] No compliance claim is made without approval.
- [ ] Stack-specific automation is deferred until stack selection.
