# Contributing

Thanks for helping improve `glue-coding-skill`.

## Good contributions

- Clearer skill instructions
- Better example prompts
- Better translations
- More precise maturity or quality-gate checks
- Small edits that make the skill easier to reuse

## Contribution guidelines

1. Keep `SKILL.md` concise. It should fit into context easily.
2. Prefer practical agent instructions over long essays.
3. Keep the mature-capability-first philosophy intact.
4. When adding a language README, keep the meaning aligned with the English README.
5. Validate the skill after editing:

```powershell
python "$env:USERPROFILE\.codex\skills\.system\skill-creator\scripts\quick_validate.py" .
```

## Pull request style

Use a short title and explain:

- what changed
- why it helps Codex write better code
- how you checked it