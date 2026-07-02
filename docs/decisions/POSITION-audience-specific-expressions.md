# Architectural Position Paper: Audience-Specific Expressions

## Status

**Proposed** — pending Evidence Review and independent adopter validation.

**Not an ADR.** Do not treat as accepted framework identity until gated review completes.

**Governance path:** Evidence Window → independent adopter evidence → Evidence Review → Entry/ADR promotion (if evidence supports).

---

## Summary

Anchor already contains repeatable engineering activities — adoption, evidence contribution, contract ownership, milestone publishing — expressed across Experience chapters, Playbooks, Reviews, Skills, and Reference Projects.

The insight is not that these activities exist. They exist implicitly.

The insight is **Audience-Specific Expressions**: the same engineering knowledge is expressed differently depending on who is consuming it and in what context.

**Practices** are the organizing mechanism — named recurring activities. They are concepts, not documents and not an eighth contract.

**Philosophy sentence:**

> A practice is the reusable engineering activity. Documentation, playbooks, skills, reviews, and reference projects are different expressions of that same practice for different audiences and purposes.

**Key distinction:** A practice is reusable engineering knowledge. Execution is what happens at runtime.

---

## Core insight

| Practice | Learning | Execution | Verification | Skill | Evidence |
|---|---|---|---|---|---|
| Project Orientation | Experience Ch. 4 | orient-project playbook | contract-ownership review | — | john-ohio journey |
| Contributing Evidence | Experience Ch. 6 · methodology | validate-through-use playbook | — | — | Evidence Window |
| Contract Ownership | Experience Ch. 3, Ch. 5 | — | contract-ownership review | what-to-keep | john-ohio sessions |

Empty cells mean no expression exists yet — not a gap to fill preemptively.

This scales beyond Anchor. It becomes a design principle for **Agentic Design Engineering**: engineering knowledge has a stable unit (the practice), with audience-specific expressions for different consumers and execution contexts. Anchor is one implementation focused on shared project understanding.

---

## Layer model

```text
Principles
        │
        ▼
Framework
        │
        ▼
Experience
        │
        ▼
Practices
        │
        ▼
Reference Projects
        │
        ▼
Independent Adoption
        │
        ▼
Evidence
        │
        ▼
Framework Evolution
```

| Layer | Question |
|---|---|
| Principles | Why? |
| Framework | What? |
| Experience | How do I learn it? |
| Practices | How do I repeatedly do it? |
| Reference Projects | What does it look like in reality? |

Reference Projects are the **proving ground** — the bridge between theory and independent adoption. They combine evidence, demonstration, teaching, and validation. Not a contract.

---

## Expression types

Audience-specific — not "human vs AI":

| Expression | Audience |
|---|---|
| Experience chapter | People learning Anchor |
| Playbook | Contributors executing a workflow |
| Review | Reviewers verifying quality |
| Skill | Specialized judgment-heavy execution |
| Reference project | Everyone through demonstration |

If, in five years, a playbook is executed by automation, an IDE extension, or a different class of tool, the concept still holds.

---

## The `ai/` directory

People reasonably assume `ai/` means "only for AI." That is not true.

Playbooks encode engineering practices. The `ai/` directory is a **location**, not an audience boundary. Playbooks are practice expressions that often serve contributors using AI tools — but the knowledge is not AI-specific.

**No rename proposed now.** Observe at Evidence Review whether independent adopters report confusion ([Handoff friction log](../../ai/handoff.md)).

---

## Newcomer journey (unchanged)

The Practices model is for **maintainers and contributors** organizing the framework — not something every user must learn upfront.

```text
Learn  →  Adopt  →  Build  →  Contribute
```

Implementation: [docs/practices/](../practices/README.md) — discoverable from CONTRIBUTING and the Contribute step, not the primary Experience chapter path.

---

## Explicit non-claims

- Eighth contract — not proposed
- Practices as a document type — practices are concepts; pages catalog expressions
- Every practice needs all expression types — empty cells are normal
- Entry §5 rewrite — deferred until Evidence Review
- Generalization to ADE — proposed as design principle, not proven across ecosystems

---

## What would support promotion to Entry/ADR

- Independent adopters find observation methodology without maintainer guidance
- Practice catalog reduces confusion about where playbooks, Experience, and evidence relate
- At least one adopter validates the model without reading this paper first
- Evidence Review concludes the model helped organize growth without documentation sprawl

---

## What would falsify this position

- Adopters ignore `docs/practices/` and continue asking "where do I start?"
- Practices model increases navigation confusion vs. the prior scattered layout
- Independent adopters report the model adds vocabulary without reducing decision budget
- Documentation volume grows faster than adoption evidence justifies

---

## Next steps

1. Ship [docs/practices/](../practices/README.md) during open Evidence Window (editorial, not structural)
2. Independent adopters contribute observations via [contributing-evidence](../practices/contributing-evidence.md)
3. Evidence Review per [governance.md](../../releases/governance.md)
4. If supported: Entry §5 evolution chain + optional ADR-004

---

## Related

- [docs/practices/README.md](../practices/README.md)
- [journey/README.md](../../journey/README.md)
- [POSITION-context-arbitration.md](POSITION-context-arbitration.md)
- [ADR-002](ADR-002-framework-vs-experience.md)
- [releases/governance.md](../../releases/governance.md)
