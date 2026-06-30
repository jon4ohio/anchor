# ADR-003: Product Narrative and Adoption (v0.2)

## Status

**Accepted**

**Date:** 2026-06-30

**Decision Maker(s):** Project maintainer

**Supersedes:** None (narrows ADR-002 Experience governance; supersedes `start-project.md` as primary adoption playbook)

---

## Context

Anchor v0.1 delivered seven contracts and a framework-first README. Adoption validation revealed strangers were sent to Project Entry before understanding value. Design discussions converged on a product strategy: responsibility-first teaching, any-project positioning, and overlay adoption (keep existing ADRs and AI context files).

ADR-002 split Framework and Experience but deferred Experience content and treated validation as research-only (`validate-through-use.md`). v0.2 ships teachable Experience content under a **teach vs. claim** rule: describe framework behavior now; normative adoption claims wait for evidence.

**In scope:** Product layers, frozen v0.2 language, responsibility-first model, adoption principle, orient-project playbook, Canonical Journey, Experience chapters, README as product page.

**Out of scope:** Eighth contract, fifth enduring principle in Entry, merging adoption and operational lifecycles in Entry §4.

---

## Decision Drivers

- Visitors must understand promise in under three minutes without reading contracts
- Majority adopters have existing docs, ADRs, and AI context — not greenfield repos
- Overlay adoption (map ownership, don't migrate files) lowers barrier vs. replacement framing
- Framework evolves from evidence; product language frozen minimally during v0.2 implementation

---

## Options Considered

### Option A: Framework-first README (status quo)

- **Description:** README points to Entry; teach contracts first.
- **Pros:** Single source of truth; simple for contributors.
- **Cons:** Wrong audience order; high bounce rate for newcomers.
- **Effort:** Low
- **Notes:** Rejected for v0.2 product layer.

### Option B: Responsibility-first product layer with frozen minimal language *(chosen)*

- **Description:** Three layers — product page (README), Experience (teach), Framework (define). Responsibility precedes contracts. Three frozen phrases. Unified `orient-project.md` playbook. Canonical Journey as teaching artifact.
- **Pros:** Matches adoption reality; teaches one question (responsibility) not seven contracts; overlay positioning.
- **Cons:** Two lifecycles to learn (adoption vs. operational); product and framework vocabulary differ slightly.
- **Effort:** Medium
- **Notes:** Operational protocol (Understand → Decide → Execute → Review → Improve) unchanged in Entry §4.

### Option C: Separate reference repository for journey

- **Description:** Canonical Journey in external repo.
- **Pros:** Cleaner meta-repo.
- **Cons:** Split attention; harder for newcomers.
- **Effort:** Medium
- **Notes:** Rejected for v0.2; in-repo `journey/john-ohio/`.

---

## Decision

**We will ship Anchor v0.2 with a responsibility-first product layer, three frozen phrases, README as product page, five Experience chapters, in-repo Canonical Journey, `orient-project.md` as unified adoption playbook, and teach-vs-claim Experience governance.**

Specifically:

1. **Frozen language (v0.2 only):** Continue instead of reconstruct; Knowledge has responsibilities; Contracts formalize responsibilities.
2. **Foundation model:** Responsibilities exist first; contracts formalize them; artifacts implement contracts.
3. **Three layers:** Product page / Experience / Framework — different audiences, no Entry duplication in README.
4. **Adoption principle:** Discover before you introduce — adoption scope, not fifth enduring principle.
5. **Teach vs. claim:** Experience describes behavior; normative claims require validation evidence.
6. **Playbooks:** `orient-project.md` for adoption; `validate-through-use.md` for research only; `start-project.md` redirects.
7. **Two lifecycles:** Adoption (Assess → Classify → Orient → Continue) documented here; operational protocol unchanged in Entry §4.
8. **Canonical Journey:** `journey/john-ohio/` — existing-project path, Session 4 continue-vs-reconstruct payoff.

---

## Consequences

### Positive

- Clear product promise before framework exposure
- Overlay adoption explicit — keep ADRs, CLAUDE.md, architecture docs
- Single adoption playbook with new/existing branches
- Responsibility question derives contracts naturally in teaching

### Negative / Trade-offs

- Contributors must maintain product layer alongside Framework
- "Orient" used as outcome; "Assess" internal to playbook — glossary documents mapping
- Experience content written before full external validation — mitigated by teach-vs-claim rule

### Operational Impact

- Release Governance layer: [releases/governance.md](../../releases/governance.md); v0.2 first instance with Evidence Window open
- Evidence Review → Decision → Next State; Major redesign not assumed
- **Migration / rollback:** Supersede with ADR if responsibility-first product layer fails evidence review

### Risks

| Risk | Likelihood | Impact | Mitigation | Owner | Review Trigger |
|------|-----------|--------|------------|-------|----------------|
| Responsibility vocabulary does not resonate with adopters | Medium | High | Log in release evidence.md; hold frozen phrases unless same confusion twice | Maintainer | Evidence Review complete for v0.2 |
| Experience mistaken for complete validated guides | Medium | Medium | Teach-vs-claim banners; no normative claims in v0.2 copy | Maintainer | User reports "misleading" twice |

---

## Review Schedule

- **Next review:** After v0.2 Evidence Review complete ([decision.md](../../releases/v0.2/decision.md))
- **Review owner:** Project maintainer

---

## Related ADRs

- [ADR-001](ADR-001-contracts-not-artifacts.md) — depends on: seven contracts, four principles
- [ADR-002](ADR-002-framework-vs-experience.md) — narrows: Experience teach-vs-claim; supersedes start-project as primary adoption path

---

## References

- [README.md](../../README.md)
- [Canonical Journey](../../journey/john-ohio/README.md)
- [Experience chapters](../../docs/experience/README.md)
- [orient-project.md](../../ai/playbooks/orient-project.md)
- [Release Governance](../../releases/README.md)
- [releases/governance.md](../../releases/governance.md)
