# Playbook: Validate Through Use

**Contract:** Playbook  
**Problem coordinated:** How do we validate Anchor on a real project without biasing results?

---

## Promise

Prescribe execution order for validating Anchor through natural project work.

---

## Prerequisites

- Anchor foundation complete on target repository (or meta-repo reference available)
- Decision to record friction, not force framework usage

---

## Research question

**Does this boundary reduce re-orientation while allowing adopting projects to evolve independently?**

Next milestone: finish a real project without feeling the need to change Anchor.

---

## Steps

### 1. Do normal work

Work on the project as you would without Anchor. Do not "try to use Anchor."

### 2. Pause when explaining

When you catch yourself re-explaining something, pause and ask:

> Which contract owns this?

If nothing owns it yet, note it. If it repeats, log it.

### 3. Create contracts only when natural

Write Specs or ADRs only when a real decision or scope boundary appears in the work—not preemptively.

### 4. Update continuity after each session

Update [Handoff](../handoff.md) delta. Add friction log rows with the Contract column filled when repetition occurs.

### 5. Log adoption observations

Track two hypotheses in the friction log—boundary pressure and contract use. Evidence, not speculation.

**Boundary — does Anchor absorb too much?**

| Observation | Possible implication |
|---|---|
| Repeated need to explain project tooling every session | Adopter documentation needs improvement, not Anchor |
| Repeated pressure to add tooling concepts to Anchor | Boundary too strict—or missing coordination concept |
| Nobody mentions tooling while using Anchor | Boundary may be invisible and working |
| No pressure to absorb tooling into Anchor | Evidence toward boundary ADR later |

**Contract — are existing contracts used?**

| Observation | Possible implication |
|---|---|
| Entry ignored; Handoff stale; decisions stay in chat | Contracts may not provide enough value |
| Specs never written when scope is bounded | Spec contract or adoption practice needs attention |
| what-to-keep never consulted; same routing mistakes repeat | Skill exemplar or contract value unclear |
| Repeated uncertainty: Handoff vs ADR vs Entry | Contract definitions may need refinement |

### 6. Run post-project review

After the project (or major phase), ask:

> What repeated coordination problem wasn't handled cleanly by the existing contracts?

Record in Handoff friction log.

### 7. Gate framework changes

Framework changes require the same friction in **two independent projects** before promotion or contract evolution.

### 8. Expand Experience content only after repetition

Experience structure exists at [docs/experience/](../../docs/experience/). Expand guide **content** only after friction log entries reveal repeated adoption questions—the Experience equivalent of "promote only after repetition."

---

## References

- [Handoff friction log](../handoff.md)
- [ADR-002: Framework vs Experience](../../docs/decisions/ADR-002-framework-vs-experience.md)
- [Project Entry](../../docs/project/entry.md)
