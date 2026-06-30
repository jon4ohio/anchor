# Contributing to Anchor

This file is **not** a framework contract. It bridges open-source collaboration with Anchor governance.

Start with [Project Entry](docs/project/entry.md) to understand the framework.

---

## How do I propose a framework change?

1. Use Anchor on a real project first—do not change the framework from theory alone.
2. Record friction in the [Handoff friction log](ai/handoff.md) with the **Contract** column filled.
3. Confirm the same friction appears in **at least two independent projects** before proposing a change.
4. Open an issue or PR describing the evidence—not the imagined benefit.

Framework changes require repeated evidence across independent projects. See [ADR-002](docs/decisions/ADR-002-framework-vs-experience.md).

---

## Proposal gate

Before proposing a framework addition or expansion, ask:

1. Would this still be true after the current session?
2. Would this still be true if the execution stack changed?
3. Does this preserve durable project context, or prescribe how adopting projects should work?

If (3) prescribes execution or tooling → adopting project documentation, not Anchor.

Both (1) and (2) must be yes for strong durable-context candidates. Either no → Handoff or adopting-project documentation.

---

## When do I write an ADR?

Write an ADR when a decision **constrains future work**—not for every implementation choice.

ADRs are immutable once accepted. To change a decision, supersede with a new ADR. See [ADR-001](docs/decisions/ADR-001-contracts-not-artifacts.md) for format.

---

## What evidence is required?

| Change type | Evidence required |
|---|---|
| New or changed contract | Same friction in two independent projects |
| Experience normative claims ("most teams…") | Same adoption question twice in validation |
| Experience descriptive content (v0.2 chapters) | Shipped under ADR-003 teach-vs-claim rule |
| New Skill, Playbook, or Review | Same workflow or question repeated twice |
| Eighth contract | Repetition proven across multiple projects—strong bar |

Record evidence in Handoff friction logs before opening PRs.

---

## What doesn't belong in Anchor?

- **Eighth contract types** without proven repetition across real projects
- **Experience normative claims** without validation evidence (descriptive teaching is allowed per ADR-003)
- **Editor-specific adapters** (Cursor rules, VS Code extensions) in the framework—those are ecosystem adapters, not Anchor
- **Decision rationale outside ADRs**, requirements outside Specs, or session state outside Handoff
- **Rewriting accepted Specs** to match later decisions—supersede or reference ADRs instead
- **Tooling, agents, MCP servers, routing tables, or prescribing how adopting projects organize their work**
- **Prescribing filenames or structure** for adopting-project documentation
- **Single-project workflow conveniences** without two-project evidence

---

## Release Governance

Anchor has three governance layers: **Framework**, **Product**, and **Release**. See [releases/governance.md](releases/governance.md).

> **During an Evidence Window, contributors record observations. Maintainers decide actions only after Evidence Review.**

**Current state:** v0.2 released. Evidence Window **open**. See [releases/v0.2/](releases/v0.2/).

### While the Evidence Window is open

- **Record** observations in [releases/v0.2/evidence.md](releases/v0.2/evidence.md) or an issue — do not open structural PRs
- **Editorial** README copy fixes are OK if meaning is unchanged
- **Structural** product or framework changes wait for Evidence Review

### Maintainer response

> We're in an Evidence Window. Please record the observation in [evidence.md](releases/v0.2/evidence.md). Changes will be considered at Evidence Review.

---

## Operations playbooks

| Playbook | When to use |
|---|---|
| [Orient Project](ai/playbooks/orient-project.md) | Adopt Anchor on any project (new or existing) |
| [Start Project](ai/playbooks/start-project.md) | Redirects to Orient Project (link stability) |
| [Validate Through Use](ai/playbooks/validate-through-use.md) | Research friction without forcing adoption |
| [Publish Foundation](ai/playbooks/publish-foundation.md) | Publish a milestone to GitHub |

---

## Questions?

New to Anchor? Start with [README](README.md) and [Experience guides](docs/experience/README.md). Contributors: [Project Entry](docs/project/entry.md), then [Handoff](ai/handoff.md).
