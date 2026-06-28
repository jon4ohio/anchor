# ADR-001: Artifacts Became Contracts

## Status

**Accepted**

**Date:** 2025-06-27

**Decision Maker(s):** Project maintainer

**Supersedes:** None

---

## Context

Anchor began as an exploration of how humans and AI can collaborate without repeatedly reconstructing project context. Early iterations framed the problem as memory, then context, then knowledge, then collaboration.

Through extended design discussion, a clearer abstraction emerged: **coordination**. Each piece of project knowledge coordinates a specific kind of work—orientation, decisions, scope, expertise, execution, quality, continuity.

The design phase produced several competing directions:

- A knowledge graph or "project brain"
- Epistemic layers tracking certainty and assumptions
- A large formal specification (800–1,200 lines)
- Seven markdown artifacts with folder conventions

The discussion converged on a simpler model: **contracts, not files**. A contract is a promise about what truth an artifact owns. The file is merely one implementation.

Additionally, "Project Brief" was renamed to **Project Entry** to reflect its function (orient a newcomer quickly) rather than its shape (a summary document). Entry is the only composite contract—it indexes other contracts without owning their content.

The design phase reached diminishing returns. Further discussion would optimize the specification without validating whether the framework works in practice.

---

## Decision

**We will freeze Anchor v0.1 as a coordination framework defined by seven contracts, four principles, and a collaboration lifecycle—and validate through usage rather than further design.**

Specifically:

1. Anchor is a **coordination framework**, not a documentation or AI framework.
2. Seven contracts: Project Entry, Specification, ADR, Skill, Playbook, Review, Handoff.
3. Four principles: contracts not files; one owner per truth; reference don't duplicate; promote only after repetition.
4. Collaboration lifecycle: Understand → Decide → Execute → Review → Improve.
5. This repository dogfoods Anchor—every contract must earn its existence by coordinating a real problem.
6. Design phase is complete. Validation begins across three projects: this meta-repo, portfolio, and greenfield.

---

## Alternatives Considered

### Option A: Continue design iteration

- **Pros:** Could resolve open questions (Skill definition, Spec lifecycle, Entry breadth) before implementation.
- **Cons:** Questions are empirical, not theoretical. Further design produces diminishing returns and delays honest failure.
- **Effort:** Low immediate; unbounded over time.

### Option B: Full formal specification (RFC, schemas, conformance tests)

- **Pros:** Precise, portable, tool-integratable.
- **Cons:** Intimidating; optimizes specification over usage; premature before three-project validation.
- **Effort:** High.

### Option C: Epistemic layers and eighth artifact types

- **Pros:** Models uncertainty explicitly; handles assumptions and provisional beliefs.
- **Cons:** Adds complexity before the seven contracts are proven sufficient. Violates "promote only after repetition."
- **Effort:** Medium.

### Option D: Freeze v0.1 and validate through usage *(chosen)*

- **Pros:** Coherent enough to fail honestly; friction reveals real gaps; matches how mature frameworks mature.
- **Cons:** Open questions remain unresolved until usage.
- **Effort:** Medium; front-loaded on dogfooding.

---

## Consequences

### Positive

- Framework can be tested immediately on real projects.
- Every weakness encountered is a real weakness, not hypothetical.
- Lean RFC lives in Project Entry (~10–20 pages), not a monolithic spec.
- Clear stopping rule for design: empirical validation across three projects.

### Negative / Trade-offs

- Skill contract definition remains experimental until portfolio validation.
- Spec lifecycle states (Draft / Active / Complete / Superseded) are suggested but not enforced in v0.1.
- No automated conformance; ownership discipline is manual.

### Operational Impact

- New contributors read [Project Entry](../project/entry.md) first, then follow the collaboration lifecycle.
- ADRs are written only for decisions that constrain future work—not every thought.
- Skills, Playbooks, and Reviews are promoted only after repetition.
- **Migration / rollback:** If validation fails, supersede this ADR with one that documents what changed and why.

### Risks

| Risk | Likelihood | Impact | Mitigation | Owner | Review Trigger |
|---|---|---|---|---|---|
| Project Entry grows into a wiki | Medium | High | Explicit must-never list; composite exception documented; run Review checklist | Maintainer | Entry exceeds ~200 lines or weekly edits |
| Skill contract proves unnecessary or wrong-shaped | Medium | Medium | Marked experimental; defer definition until portfolio | Maintainer | After portfolio validation |
| Framework ignored in favor of chat context | Medium | High | Handoff + friction log track repeated explanations | Maintainer | Same explanation twice in one project |

---

## Related ADRs

N/A — no known relationships.

---

## References

- [Project Entry](../project/entry.md) — Anchor v0.1 framework definition
- Design conversation leading to coordination framework abstraction
