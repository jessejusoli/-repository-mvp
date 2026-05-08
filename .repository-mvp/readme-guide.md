# README Guide

Use this guide to turn the root `README.md` into the best first entry point for the project. The README should help a new reader understand what the project is, why it exists, how to start, where to go next, and how trustworthy the repository is.

## README Goal

The README is not a full documentation site. It is the front door.

It should answer:

- what this project is;
- who it is for;
- what problem it solves;
- what the current version is trying to achieve;
- how to install, run, use, test, or evaluate it once the stack exists;
- where deeper documentation lives;
- how humans and AI agents should safely contribute.

## Recommended First Screen

Keep the first screen useful without making it noisy:

1. project name;
2. badges;
3. one-sentence purpose;
4. concise project snapshot;
5. start-here links.

The current root `README.md` already includes starter badges for template status, living docs, AI agents, and proprietary license. Replace or expand them after the project identity and GitHub repository path are known.

## Badges

Badges are useful when they communicate real status. Avoid badges that look impressive but do not help the reader make a decision.

Useful badge categories:

- license;
- project status;
- CI/CD status;
- documentation status;
- current release;
- package version;
- security scan status;
- coverage, only if coverage is meaningful;
- GitHub stars and forks for public projects.

Example static badges:

```md
[![Status](https://img.shields.io/badge/status-mvp-blue)](#project-snapshot)
[![Docs](https://img.shields.io/badge/docs-living-brightgreen)](docs/README.md)
[![License](https://img.shields.io/badge/license-proprietary-lightgrey)](LICENSE.md)
```

Example GitHub badges:

```md
[![CI](https://github.com/[GITHUB_OWNER]/[GITHUB_REPOSITORY]/actions/workflows/repository-hygiene.yml/badge.svg)](https://github.com/[GITHUB_OWNER]/[GITHUB_REPOSITORY]/actions/workflows/repository-hygiene.yml)
[![Stars](https://img.shields.io/github/stars/[GITHUB_OWNER]/[GITHUB_REPOSITORY]?style=social)](https://github.com/[GITHUB_OWNER]/[GITHUB_REPOSITORY]/stargazers)
[![Forks](https://img.shields.io/github/forks/[GITHUB_OWNER]/[GITHUB_REPOSITORY]?style=social)](https://github.com/[GITHUB_OWNER]/[GITHUB_REPOSITORY]/forks)
[![Issues](https://img.shields.io/github/issues/[GITHUB_OWNER]/[GITHUB_REPOSITORY])](https://github.com/[GITHUB_OWNER]/[GITHUB_REPOSITORY]/issues)
```

## Images

Use images when they clarify the project faster than text.

Good uses:

- product screenshots;
- architecture diagrams;
- workflow diagrams;
- terminal output screenshots only when text output is not enough;
- before-and-after comparisons;
- feature previews.

Recommended pattern:

```md
![Short accessible description](docs/assets/[IMAGE_FILE].png)
```

For controlled sizing on GitHub, HTML image tags are acceptable:

```html
<img src="docs/assets/[IMAGE_FILE].png" alt="Short accessible description" width="720">
```

Image rules:

- keep images in a predictable folder such as `docs/assets/`;
- use descriptive filenames;
- include meaningful alt text;
- compress large images;
- avoid decorative images that do not explain the project.

## Videos

Use videos for demos, setup walkthroughs, and workflow previews. GitHub README rendering is more reliable when the README links to a video or uses an image thumbnail that links to the video.

Recommended pattern:

```md
[![Demo video](docs/assets/[VIDEO_THUMBNAIL].png)]([VIDEO_URL])
```

Video rules:

- keep the thumbnail clear and current;
- link to a stable hosted video or GitHub release asset;
- include a short text summary near the link;
- do not rely on video as the only documentation for a workflow.

## Links

Use links to keep the README concise while preserving depth.

Good README links:

- documentation index;
- architecture guide;
- API documentation;
- changelog;
- backlog and task manager;
- contribution or agent instructions;
- releases;
- issues;
- discussions;
- security policy, once it exists.

Prefer relative links for files inside the repository:

```md
[Architecture](docs/architecture.md)
```

Use absolute GitHub links for repository features:

```md
[Releases](https://github.com/[GITHUB_OWNER]/[GITHUB_REPOSITORY]/releases)
[Issues](https://github.com/[GITHUB_OWNER]/[GITHUB_REPOSITORY]/issues)
[Discussions](https://github.com/[GITHUB_OWNER]/[GITHUB_REPOSITORY]/discussions)
```

## Lists, Tables, And Quotes

Use lists for sequence and scanning:

```md
1. Install dependencies.
2. Configure environment variables.
3. Run checks.
```

Use tables for compact facts:

```md
| Area | Value |
| --- | --- |
| Status | MVP |
| Owner | [OWNER] |
```

Use blockquotes for short warnings, notes, or cited statements:

```md
> This repository starts as proprietary until the owner intentionally selects another license.
```

Do not use blockquotes for long documentation. Move long content into `docs/` and link to it.

## Citations And References

Use citations when the README depends on a standard, paper, external API, legal requirement, vendor document, or benchmark. Prefer references near the relevant statement instead of a loose list of links at the bottom.

Reference-style links keep paragraphs readable:

```md
This project follows the selected API contract standard described in [REFERENCE_TITLE][reference-id].

[reference-id]: [REFERENCE_URL]
```

Footnotes are useful for short context notes:

```md
The first production release must define a public API compatibility policy.[^api-policy]

[^api-policy]: Replace this with the selected API policy reference and access date.
```

Citation rules:

- cite primary sources when possible;
- include access dates for external references that may change;
- do not cite sources the project has not actually used;
- keep legal, medical, financial, and compliance references current.

## GitHub-Flavored Markdown Features

GitHub README files can use helpful repository-native syntax:

```md
- [ ] Pending task
- [x] Completed task

Related issue: #123
Related pull request: #456
Maintainer: @GITHUB_USERNAME
Commit: abc1234
```

Use these features when they point to real repository activity. Avoid permanent README links to temporary planning issues unless the issue is part of the public project record.

## GitHub Repository Signals

GitHub already shows stars, forks, watchers, issues, pull requests, releases, packages, deployments, and repository metadata around the README. The README should link to the most useful signals when they help the project audience.

Useful links for public projects:

```md
- [Star this repository](https://github.com/[GITHUB_OWNER]/[GITHUB_REPOSITORY]/stargazers)
- [Fork this repository](https://github.com/[GITHUB_OWNER]/[GITHUB_REPOSITORY]/fork)
- [Open issues](https://github.com/[GITHUB_OWNER]/[GITHUB_REPOSITORY]/issues)
- [Releases](https://github.com/[GITHUB_OWNER]/[GITHUB_REPOSITORY]/releases)
```

Use these only when they match the project purpose. A private internal project may not need star or fork links.

## README Quality Checklist

- [ ] The first paragraph explains the project in one sentence.
- [ ] Badges show real, useful repository status.
- [ ] Links point to existing files or stable external pages.
- [ ] Images have alt text and are stored predictably.
- [ ] Videos are linked through a stable thumbnail or URL.
- [ ] Setup and usage instructions are present once the stack exists.
- [ ] The README links to `AGENTS.md`, `VERTICAL.md`, `CHANGELOG.md`, and `docs/`.
- [ ] The README stays concise and moves details to `docs/`.
- [ ] No secrets, private URLs, or internal-only screenshots are exposed.
- [ ] The README is updated in the same change as major project behavior or structure changes.
