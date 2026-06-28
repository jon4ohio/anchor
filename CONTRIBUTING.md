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

## When do I write an ADR?

Write an ADR when a decision **constrains future work**—not for every implementation choice.

ADRs are immutable once accepted. To change a decision, supersede with a new ADR. See [ADR-001](docs/decisions/ADR-001-contracts-not-artifacts.md) for format.

---

## What evidence is required?

| Change type | Evidence required |
|---|---|
| New or changed contract | Same friction in two independent projects |
| Experience guide content | Same adoption question twice in validation |
| New Skill, Playbook, or Review | Same workflow or question repeated twice |
| Eighth contract | Repetition proven across multiple projects—strong bar |

Record evidence in Handoff friction logs before opening PRs.

---

## What doesn't belong in Anchor?

- **Eighth contract types** without proven repetition across real projects
- **Experience content written from theory** before validation (structure is fine; content waits for evidence)
- **Editor-specific adapters** (Cursor rules, VS Code extensions) in the framework—those are ecosystem adapters, not Anchor
- **Decision rationale outside ADRs**, requirements outside Specs, or session state outside Handoff
- **Rewriting accepted Specs** to match later decisions—supersede or reference ADRs instead

---

## Operations playbooks

| Playbook | When to use |
|---|---|
| [Start Project](ai/playbooks/start-project.md) | Initialize Anchor on a new repository |
| [Validate Through Use](ai/playbooks/validate-through-use.md) | Validate on an existing project |
| [Publish Foundation](ai/playbooks/publish-foundation.md) | Publish a milestone to GitHub |

---

## Questions?

Read [Project Entry](docs/project/entry.md), then [Handoff](ai/handoff.md) for current state.
