# Skill: Distillation

**Contract:** Skill *(experimental)*  
**Status:** Probe — not a canonical template  
**Problem coordinated:** How do conversations become durable knowledge?

---

## Promise

Teach how to promote recurring insights from conversation into the correct contract.

---

## Why This Exists

This problem recurred throughout Anchor's design phase: valuable ideas emerged in chat but had no durable home. The same explanations were given multiple times across sessions. That repetition satisfies "promote only after repetition" for this meta-repo.

**The Skill contract itself remains experimental.** This file is a probe to test whether expertise-style guidance works. After portfolio validation, we will know whether a Skill is a methodology, reusable expertise, or something else.

---

## Principles

1. **Conversation is raw material, not storage.** Chat is transient. Contracts are durable.
2. **Route by question type, not by importance.** The recurring question determines the contract—not how significant the idea feels.
3. **When in doubt, Handoff.** Provisional insights stay in Handoff until repetition proves they need a contract.

---

## Rules

| If people keep asking… | Promote to… | Not to… |
|---|---|---|
| Why did we choose this? | ADR | Entry, Spec |
| What are we building? | Spec | Entry, ADR |
| How do we do this kind of work? | Skill | Playbook, Review |
| What steps do we follow? | Playbook | Skill |
| Is this good enough? | Review | Skill, Playbook |
| What changed / what's next? | Handoff | Entry, Spec |
| What is this project? | Entry | Everywhere else |

Apply the inclusion test before promoting: does another contract already own this truth?

---

## Example

**Conversation insight:** "We realized Anchor isn't about memory—it's about coordination."

**Wrong placement:** Add paragraph to Project Entry (Entry owns identity, not decision rationale).

**Right placement:** Record in ADR-001 as context for the decision to freeze v0.1 as a coordination framework. Entry references the ADR in its index.

---

## Must Never Contain

- Project-specific requirements (see Specs)
- Sequential workflow steps (see Playbooks)
- Pass/fail checklists (see Reviews)

---

## Open Questions (deferred)

- Is a Skill portable across all projects, or partially project-specific?
- Should Skills live inside the repo or in a personal/org library?
- How does a Skill differ from a Playbook in practice when both involve "how to"?

Answer through portfolio and greenfield validation—not design discussion.
