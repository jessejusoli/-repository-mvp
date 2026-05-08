# Release Process

This file defines how `[PROJECT_NAME]` versions and ships changes. It does not replace [../CHANGELOG.md](../CHANGELOG.md).

## Release Boundaries

- Planned future direction belongs in [../ROADMAP.md](../ROADMAP.md).
- Current version focus belongs in [../VERTICAL.md](../VERTICAL.md).
- Completed notable changes belong in [../CHANGELOG.md](../CHANGELOG.md).
- Release process and readiness belong here.

## Versioning

Versioning model: `[VERSIONING_MODEL]`

Use semantic versioning once the project has a stable public interface, unless the owner documents another model.

## Release Checklist

- [ ] Scope matches the current vertical goal.
- [ ] Requirements and acceptance criteria are satisfied.
- [ ] Required checks passed.
- [ ] Security review is complete when required.
- [ ] Documentation is updated.
- [ ] Changelog is updated.
- [ ] Version tag or release identifier is prepared.
- [ ] Rollback or recovery path is documented when applicable.

## Release Notes Template

```md
## [VERSION] - [YYYY-MM-DD]

### Summary

[RELEASE_SUMMARY]

### Changes

- [CHANGE]

### Compatibility

[COMPATIBILITY_NOTES]

### Upgrade Or Rollback

[UPGRADE_OR_ROLLBACK_NOTES]
```

## Rollback Guidance

Rollback strategy: `[ROLLBACK_STRATEGY]`

Define a concrete rollback path before releasing anything that affects users, data, infrastructure, or public interfaces.
