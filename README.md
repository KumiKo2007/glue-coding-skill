<p align="center">
  <strong>README</strong> ·
  <a href="CODE_OF_CONDUCT.md">Code of conduct</a> ·
  <a href="CONTRIBUTING.md">Contributing</a> ·
  <a href="LICENSE">MIT license</a> ·
  <a href="SECURITY.md">Security</a>
</p>

<p align="center">
  <a href="README.md"><strong>English</strong></a> ·
  <a href="README.zh-CN.md">中文</a> ·
  <a href="README.ja.md">日本語</a> ·
  <a href="README.ko.md">한국어</a>
</p>

<p align="center">
  <span style="font-size:48px">🧩</span>
</p>

<h1 align="center">glue-coding-skill: Build With Leverage, Not Reinvention</h1>

<p align="center"><strong>A Codex skill for AI coding workflows: reuse mature capabilities, write thin glue code, add quality gates, and leave a replacement path.</strong></p>

<hr />

<p align="center">
  <a href="LICENSE"><img alt="License MIT" src="https://img.shields.io/badge/license-MIT-2ea44f?style=for-the-badge"></a>
  <img alt="Codex Skill" src="https://img.shields.io/badge/Codex-Skill-111827?style=for-the-badge">
  <img alt="AI Coding" src="https://img.shields.io/badge/AI%20Coding-Workflow-2563eb?style=for-the-badge">
  <img alt="Languages" src="https://img.shields.io/badge/Languages-EN%20%7C%20ZH%20%7C%20JA%20%7C%20KO-f59e0b?style=for-the-badge">
</p>

<p align="center">
  <a href="#why-this-skill-exists"><img alt="Why" src="https://img.shields.io/badge/why-this%20exists-374151"></a>
  <a href="#what-it-does"><img alt="What it does" src="https://img.shields.io/badge/what-it%20does-7c3aed"></a>
  <a href="#install"><img alt="Install" src="https://img.shields.io/badge/install-0ea5e9"></a>
  <a href="#example-prompts"><img alt="Prompts" src="https://img.shields.io/badge/example-prompts-dc2626"></a>
  <a href="SKILL.md"><img alt="Skill" src="https://img.shields.io/badge/SKILL.md-open-111827"></a>
</p>

<p align="center">
  <a href="#mature-capability-first"><img alt="Mature capability first" src="https://img.shields.io/badge/mature--capability-first-16a34a"></a>
  <a href="#thin-glue-layer"><img alt="Thin glue layer" src="https://img.shields.io/badge/thin-glue%20layer-0891b2"></a>
  <a href="#quality-gates"><img alt="Quality gates" src="https://img.shields.io/badge/quality-gates-9333ea"></a>
  <a href="#replacement-path"><img alt="Replacement path" src="https://img.shields.io/badge/replacement-path-f97316"></a>
</p>

<p align="center">
  <a href="README.zh-CN.md">中文介绍</a> ·
  <a href="README.ja.md">日本語紹介</a> ·
  <a href="README.ko.md">한국어 소개</a>
</p>

## Why this skill exists

AI can write a lot of code very quickly. That is useful, but it also makes it easy to accidentally rebuild authentication, queues, schedulers, SDK wrappers, logging systems, storage layers, or private platforms.

`glue-coding` gives Codex a simple engineering instinct:

> Mature capabilities solve common problems. Glue code connects business flows. Custom core code is the exception, not the default.

## What it does

This skill guides Codex to:

- search for official SDKs, APIs, frameworks, managed services, and stable open-source tools first
- draw a clean boundary between domain logic and integration details
- keep custom code short, testable, observable, reversible, and easy to delete
- add quality gates before accepting an integration as done
- explain why custom core code is necessary when reuse is not enough

## Core loop

```text
Intent -> Mature capability search -> Option evaluation -> Boundary design
       -> Thin glue layer -> Quality gates -> Replacement or rollback path
       -> Recursive refinement
```

## Mature capability first

Before writing custom code, Codex should ask:

1. Does an official or well-maintained capability already solve this?
2. Is the cost, risk, license, and operational burden acceptable?
3. Can the business logic stay clean if this dependency changes?

## Thin glue layer

Good glue code adapts, orchestrates, validates, and isolates. It should not quietly become a second framework.

## Quality gates

The skill pushes for tests, schema checks, error handling, retries, observability, and clear acceptance criteria around integration points.

## Replacement path

Every external dependency should have a known replacement, rollback, or deletion story. If the dependency fails, the business model should not be trapped inside it.

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
- "Use glue-coding to refactor this module so business logic stays clean and the integration stays thin."
- "Use glue-coding to find the smallest replaceable implementation for this workflow."

## Good fit

- feature planning
- architecture review
- refactoring AI-generated code
- API and SDK integration
- workflow orchestration
- deciding whether to build, buy, wrap, or delete

## Not the goal

This is not anti-custom-code. It is a bias toward engineering leverage. When custom code is truly the right choice, the skill asks Codex to name the reason, define the boundary, and leave a future replacement path.

## License

MIT.