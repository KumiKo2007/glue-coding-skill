# Security Policy

This repository contains a Codex skill, not executable application code. Still, security matters because skills shape agent behavior.

## Supported versions

The `main` branch is the supported version.

## Reporting security issues

Please open a GitHub issue if the skill encourages unsafe behavior, insecure dependency use, secret leakage, or risky automation patterns.

Avoid posting real secrets, private tokens, or sensitive production details in public issues.

## Security principles for this skill

- Prefer official and maintained dependencies.
- Avoid custom security primitives.
- Keep external integrations isolated from domain logic.
- Require testing, rollback, and replacement paths for dependencies.