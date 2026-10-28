# AGENTS.md

## Versioning

Whenever you commit, update the version numbers:

- Bump `version` in `.claude-plugin/plugin.json` of every plugin the commit changes.
- Bump `metadata.version` in `.claude-plugin/marketplace.json`.
- Use semver: fix → patch, feature → minor, breaking change → major.
- While developing toward a version, add a numbered `-pre.N` suffix: start at `-pre.1` (e.g. `0.1.0-pre.1`), then `-pre.2`, `-pre.3`, … on every commit, so each change gets a new version and updates are picked up.
- Same for the marketplace (e.g. `1.1.0-pre.1`, `1.1.0-pre.2`, …).
- On release, drop the suffix (e.g. `0.1.0`).
