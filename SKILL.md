---
name: glue-coding
description: Prefer mature, verified capabilities over rebuilding core systems. Use when designing, reviewing, or implementing code that should reuse existing SDKs, APIs, frameworks, platform services, or open-source components, and when deciding whether to build a thin glue layer instead of core infrastructure.
---

# Glue Coding

Use this skill to turn coding work into an integration problem: find mature capabilities first, keep custom code thin, and make every non-core choice replaceable.

## Core Rules

- Prefer official SDKs, platform services, maintained libraries, and proven standards.
- Treat self-written code as glue unless a new core capability is truly required.
- Do not rebuild auth, payments, queues, schedulers, logging, storage, observability, or model wrappers when a mature option fits the constraints.
- Require a clear boundary between core business logic and external dependencies.
- Optimize for testability, observability, reversibility, and deletion.

## Workflow

1. Clarify the business goal, inputs, outputs, constraints, and acceptance criteria.
2. Find mature options first: official docs, production-used libraries, managed services, or internal shared components.
3. Evaluate each candidate for maintenance status, docs, versioning, test coverage, production evidence, migration risk, security, and cost.
4. Draw the boundary: keep domain rules inside, keep integration details outside, and isolate every external dependency.
5. Implement the thinnest possible glue layer.
6. Add tests, schema checks, retries, fallbacks, and monitoring for the integration points.
7. State the replacement path before calling it done.

## Recursive Refinement

- After the first working version, ask again whether any custom logic can be replaced by a mature capability.
- Tighten boundaries until the glue code is short, clear, and easy to remove.
- If a custom core still remains, justify it explicitly with constraints, risk, or missing mature alternatives.
- Repeat the evaluation whenever the integration surface changes.

## Mature Capability Checklist

Prefer:

- Official SDKs and APIs
- Maintained open-source packages
- Managed services
- Stable platform features
- Public standards and protocols
- Internal shared services with real production use

Evaluate:

- Maintenance status
- Release cadence and versioning
- Documentation quality
- Test coverage and CI
- Production evidence
- Security and compliance fit
- Migration and rollback cost
- Operational overhead

Common self-build traps:

- Authentication and authorization
- Payments and billing
- Queues and scheduling
- Logging, tracing, and metrics
- Storage and persistence primitives
- Model or API wrapper layers
- Retry, backoff, and circuit breaking

Before writing custom code:

1. Is there a mature capability that already does this?
2. Can the business logic stay separate from the integration layer?
3. Can the dependency be swapped without rewriting the core?
4. Can the result be tested and observed directly?
5. Is the custom code actually smaller than the mature alternative?

