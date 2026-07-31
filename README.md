# Glue Coding Skill

Build with leverage, not reinvention.

`glue-coding` is a single-file Codex skill for AI-assisted engineering. It teaches the agent to stop inventing core systems from scratch, search for mature capabilities first, and write only the thin integration layer that turns those capabilities into a working business flow.

Use it when vibe coding starts to feel too magical: APIs appear from nowhere, frameworks get rebuilt accidentally, and "just one wrapper" quietly becomes a private platform.

## The idea

Modern AI coding is strongest when it connects proven pieces well. This skill gives Codex a small but stubborn engineering instinct:

> Mature capabilities solve common problems. Glue code connects business flows. Custom core code is the exception, not the default.

## What it helps with

- Choosing SDKs, APIs, frameworks, and managed services before custom code
- Drawing a clean boundary between domain logic and integration glue
- Avoiding the classic trap of rebuilding auth, queues, billing, logging, or wrappers
- Turning the first working version into a smaller, more maintainable one
- Asking for a replacement or rollback path before the design feels "done"

## What is inside

- [`SKILL.md`](SKILL.md): the complete skill, ready to copy or clone
- A mature capability checklist for evaluating reuse options
- A recursive refinement loop for shrinking unnecessary custom code
- Practical guardrails for SDKs, APIs, queues, auth, logging, storage, and AI wrappers

## Install

Clone this repo into your Codex skills directory:

```powershell
git clone https://github.com/KumiKo2007/glue-coding-skill "$env:USERPROFILE\.codex\skills\glue-coding"
```

Or manually create a folder named `glue-coding` in your skills directory and put [`SKILL.md`](SKILL.md) inside it.

Then ask Codex to use it:

```text
Use $glue-coding to design this feature with mature capabilities first.
```

## Example prompts

- "Use glue-coding to decide whether we should wrap this SDK or write our own integration layer."
- "Use glue-coding to review this feature and tell me what should be reused instead of rebuilt."
- "Use glue-coding to refactor this module so the business logic stays clean and the integration is thin."
- "Use glue-coding to find the smallest replaceable implementation for this workflow."

## Good fit

- Feature planning
- Architecture review
- Refactoring AI-generated code
- API and SDK integration
- Workflow orchestration
- Deciding whether to build, buy, wrap, or delete

## Not the goal

This skill is not a low-code manifesto and it is not anti-custom-code. It is a bias toward engineering leverage. When custom code is truly the right choice, the skill asks the agent to name the reason, define the boundary, and leave a future replacement path.

## Why this skill exists

Most coding time is not spent inventing new primitives. It is spent connecting proven ones without letting the glue become a second product. This skill keeps that work explicit and repeatable, especially when AI can write a lot of code very quickly.

If your AI coding sessions often produce too much code, too many homemade abstractions, or suspiciously confident integrations, this skill is meant to add a little engineering gravity.

## License

MIT.