# Playbook: Orient Project

**Contract:** Playbook  
**Problem coordinated:** How do we adopt Anchor on any project?

---

## Promise

Prescribe execution order for orienting a project — new or existing — into Anchor's responsibility model without unnecessary migration.

Executes the adoption process in [Adopt Anchor](../../docs/experience/04-building-your-own.md).

---

## Prerequisites

- Git repository (empty or mature)
- Willingness to map ownership before creating new structure
- If someone else is executing this playbook for you, see [Delegating adoption](../../docs/experience/04-building-your-own.md#delegating-adoption)

---

## Steps

### 1. Assess current project state

Understand the project as it exists today.

Determine project state:

- [ ] **New project** — little exists yet → [Branch A](#branch-a-new-project)
- [ ] **Existing project** — docs, ADRs, AI context, or conventions already exist → [Branch B](#branch-b-existing-project)

---

### Branch A: New project

#### 2a. Classify — initial responsibilities

Identify first real work. Which responsibilities will you need?

- Project identity → Entry
- First bounded scope → Spec
- Decisions that constrain work → ADR (when they arise)

#### 3a. Orient — establish owners

Create Project Entry. Include purpose, where truths will live, pointer to framework if using Anchor contracts.

Keep [README](../../README.md) as product page for visitors — not a duplicate of Entry.

Create first Spec for initial work. Skip ADR until a decision constrains future work.

#### 4a. Review

Run [contract-ownership Review](../reviews/contract-ownership.md) on new contract files.

#### 5a. Handoff

Write or update Handoff. Record delta, horizon, blocks.

---

### Branch B: Existing project

#### 2b. Classify — map responsibilities

Inventory artifacts that coordinate the project (README, ADRs, architecture docs, `CLAUDE.md`, specs, notes).

For each artifact ask:

> What responsibility does this knowledge have?

| Responsibility | Contract |
|----------------|----------|
| Project identity | Entry |
| Decision | ADR |
| Intended behavior | Spec |
| Expertise | Skill |
| Quality | Review |
| Procedure | Playbook |
| Session continuity | Handoff |

Files may not move. Ownership clarifies.

Pay special attention to AI context files (`CLAUDE.md`, `AGENTS.md`, etc.) that mix identity, expertise, and session state.

#### 3b. Orient — map and fill gaps only

- Map existing artifacts to contract owners
- Create contracts only where no owner exists
- Trim duplication — reference owners instead of restating rationale
- Add or update Entry as index of where truths live

#### 4b. Review

Run [contract-ownership Review](../reviews/contract-ownership.md) on affected contract files.

#### 5b. Handoff

Write or update Handoff. Record what was mapped, what gaps were filled, horizon, blocks.

---

### 6. Continue

Normal work. Update Handoff between sessions. Promote repeated knowledge per [what-to-keep Skill](../skills/what-to-keep.md).

Continue instead of reconstruct.

---

## After orientation

Apply the post-project review question after each significant effort:

> What repeated coordination problem wasn't handled cleanly by the existing contracts?

Record answers in Handoff friction log.

For **research** validation (observing friction without forcing adoption), see [Validate Through Use](validate-through-use.md) — not a substitute for this playbook.

---

## References

- [Practice: Project Orientation](../../docs/practices/project-orientation.md)
- [Adopt Anchor](../../docs/experience/04-building-your-own.md)
- [Canonical Journey](../../journey/john-ohio/README.md)
- [Project Entry](../../docs/project/entry.md)
- [what-to-keep Skill](../skills/what-to-keep.md)
- [contract-ownership Review](../reviews/contract-ownership.md)
