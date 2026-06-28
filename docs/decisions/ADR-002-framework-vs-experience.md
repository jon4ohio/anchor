# ADR-002: Framework vs Experience

## Status

**Accepted**

**Date:** 2026-06-28

**Decision Maker(s):** Project maintainer

**Supersedes:** None

---

## Context

Anchor v0.1 foundation is complete locally: seven contracts, four principles, passing ownership audit, self-hosting meta-repo. The design phase reached diminishing returns in ADR-001.

Two tensions emerged during refinement:

1. **Adoption is a product.** Quick Start, Using Anchor, and Examples are not framework contracts—they teach the system. They deserve a distinct place without polluting the seven-contract model.

2. **Language matters.** "Bootstrap" is technically correct but requires specialist knowledge. Contributors think "start a project" and "foundation complete," not "bootstrap."

Additionally, Experience documentation written before validation would be theoretical. Experience structure can exist early; content must emerge from observed adoption friction.

**In scope:** Product split, naming, Experience governance, validation methodology, friction log shape, version vs milestone semantics.

**Out of scope:** Eighth contract, CLI, editor adapters, full Experience content.

---

## Decision Drivers

- Framework must remain AI-compatible but AI-independent
- Experience docs must not become a second framework or wiki
- Version tags must stay semantic; milestone names stay human-readable
- Framework evolves only from evidence, not anticipation
- Repository should have complete product shape before validation begins

---

## Options Considered

### Option A: Single product — all docs are framework

- **Description:** Treat Quick Start and guides as extensions of Project Entry or new contract types.
- **Pros:** Simple structure; one index.
- **Cons:** Blurs contract ownership; Entry becomes a wiki; violates one owner per truth.
- **Effort:** Low
- **Notes:** Rejected — adoption teaching is not orientation.

### Option B: Two products with parallel validation and Experience tracks

- **Description:** Build Experience guides while validating on portfolio.
- **Pros:** Faster perceived onboarding.
- **Cons:** Guides written from theory, not evidence; duplicates Skills/Playbooks governance violation in spirit.
- **Effort:** Medium
- **Notes:** Rejected — Experience content must follow validation.

### Option C: Two products, scaffold Experience early, expand after validation *(chosen)*

- **Description:** Framework defines the system; Experience teaches it. Minimal Experience scaffolding establishes product shape. Content expands only after repeated adoption questions. Foundation is a milestone; Git tags use semantic versioning (`v0.1.0-foundation`).
- **Pros:** Complete repository shape; evidence-first content; clear governance mirror; approachable language.
- **Cons:** Placeholder docs may feel incomplete until validation fills them.
- **Effort:** Medium
- **Notes:** Matches Skill probe pattern from meta-repo.

---

## Decision

**We will treat Anchor as two products—Framework (seven contracts) and Experience (adoption docs)—scaffold Experience structure during foundation, expand Experience content only after repeated adoption questions in validation, rename bootstrap terminology to foundation/start-project language, and use semantic Git tags with human release titles.**

Specifically:

1. **Framework** owns coordination contracts. **Experience** owns adoption documentation at `docs/experience/`.
2. **Governance mirror:** Framework promotes after repeated evidence across independent projects. Experience expands after repeated adoption questions.
3. **Milestone:** Foundation Complete. **Tag:** `v0.1.0-foundation`. **Release title:** Anchor Foundation.
4. **`bootstrap-project.md` → `start-project.md`**, title **Start Project**.
5. **Friction log** gains a **Contract** column; remove Framework failure? column.
6. **Validation** uses natural work—not forced framework usage. Pause when explaining; ask which contract owns it.
7. **Glossary** at `docs/experience/glossary.md` — stable vocabulary reference for newcomers.

---

## Consequences

### Positive

- Clear boundary between defining and teaching the system
- Repository has complete product shape before portfolio validation
- Semantic versioning scales (`v0.2.0-validation`, `v1.0.0`)
- User-facing language matches mental models
- Friction log ties improvements to existing contracts

### Negative / Trade-offs

- Experience placeholders feel minimal until validation fills them
- Two governance rules to remember (framework vs Experience)
- ADR-001 still says "bootstrap" in places — immutable; this ADR supersedes naming going forward

### Operational Impact

- No framework changes without evidence from at least two independent projects
- Experience README/quick-start/using-anchor/examples expand after friction; glossary evolves with vocabulary
- Handoff carries operational roadmap only—not framework definition
- **Migration / rollback:** Supersede with ADR documenting reversion if two-product split fails validation

### Risks

| Risk | Likelihood | Impact | Mitigation | Owner | Review Trigger |
|------|-----------|--------|------------|-------|----------------|
| Experience placeholders mistaken for complete guides | Medium | Medium | Banner on every Experience doc stating validation-phase minimal status | Maintainer | User confusion reported twice |
| Handoff roadmap becomes second Entry | Low | High | Roadmap limited to version state, active phase, out of scope; guardrail in Handoff | Maintainer | Roadmap exceeds 8 lines or restates principles |

---

## Review Schedule

- **Next review:** After portfolio and greenfield validation complete
- **Review owner:** Project maintainer

---

## Related ADRs

- [ADR-001](ADR-001-contracts-not-artifacts.md) — depends on: seven contracts, freeze v0.1, validate through usage

---

## References

- [Project Entry](../project/entry.md)
- [Handoff](../../ai/handoff.md)
- Foundation refinement plan (2026-06-28)
