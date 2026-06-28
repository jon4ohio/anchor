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

### 5. Run post-project review

After the project (or major phase), ask:

> What repeated coordination problem wasn't handled cleanly by the existing contracts?

Record in Handoff friction log.

### 6. Gate framework changes

Framework changes require the same friction in **two independent projects** before promotion or contract evolution.

### 7. Expand Experience content only after repetition

Experience structure exists at [docs/experience/](../../docs/experience/). Expand guide **content** only after friction log entries reveal repeated adoption questions—the Experience equivalent of "promote only after repetition."

---

## References

- [Handoff friction log](../handoff.md)
- [ADR-002: Framework vs Experience](../../docs/decisions/ADR-002-framework-vs-experience.md)
- [Project Entry](../../docs/project/entry.md)
