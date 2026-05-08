# Project Documentation

This directory contains the living documentation for `[PROJECT_NAME]`.

## User Guide

`[USER_GUIDE_OVERVIEW]`

Describe the primary user workflow:

1. `[USER_STEP_1]`
2. `[USER_STEP_2]`
3. `[USER_STEP_3]`

## Documentation Map

- [Documentation system and anti-duplication rules](documentation-system.md)
- [Requirements](requirements.md)
- [Compliance readiness](compliance.md)
- [Architecture and decision guidance](architecture.md)
- [API documentation guidance](api.md)
- [Automation guidance](automation.md)
- [Quality](quality.md)
- [Release process](release.md)
- [Operations readiness](operations.md)
- [Glossary](glossary.md)
- [Risk register](risk-register.md)

## Documentation Standards

- Keep documentation close to the behavior it describes.
- Update documentation in the same change that modifies user workflows, architecture, operations, or public interfaces.
- Prefer concise pages with clear links over duplicated long-form explanations.
- Use [documentation-system.md](documentation-system.md) to avoid duplicate sources of truth.
- Keep en-US as the source language.
- Add translations under folders such as `docs/pt-BR/` only when requested.

## Project Overview

| Area | Current Value |
| --- | --- |
| Product or system | `[PROJECT_NAME]` |
| Audience | `[PRIMARY_AUDIENCE]` |
| Main workflow | `[MAIN_WORKFLOW]` |
| Operational owner | `[OPERATIONAL_OWNER]` |
| Support channel | `[SUPPORT_CHANNEL]` |

## Definition of Ready

A change is ready to implement when:

- the expected outcome is clear;
- the affected docs are known;
- the relevant task is listed in [TASK_MANAGER.md](../TASK_MANAGER.md);
- the work supports the current vertical goal.

## Definition of Done

A change is done when:

- implementation or documentation has been completed;
- relevant checks have passed;
- affected living documentation has been updated;
- [CHANGELOG.md](../CHANGELOG.md) has been updated when project behavior, structure, or interfaces changed.
