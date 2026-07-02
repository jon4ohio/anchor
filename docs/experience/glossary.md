# Glossary

> **Product documentation — not a framework contract.**

---

## Frozen phrases (v0.2)

**Continue instead of reconstruct.** — Anchor's transformation slogan.

**Knowledge has responsibilities.** — Different kinds of project knowledge do different jobs.

**Contracts formalize responsibilities.** — Named owners for each responsibility type.

---

## Product terms

**Adopt Anchor** — [Experience Chapter 4](04-building-your-own.md); how to bring Anchor to your project.

**Canonical Journey** — [John Ohio's walkthrough](../../journey/john-ohio/README.md); the canonical teaching artifact for Anchor v0.2.

**Product page** — [README.md](../../README.md); discover and evaluate before adopting.

**Experience** — Adoption documentation in this directory. Not a contract.

**Framework** — Seven contracts defined in [Project Entry](../project/entry.md).

---

## Adoption terms

**Responsibility** — The job a piece of knowledge performs (identity, decision, session state, etc.). Ask: *What responsibility does this knowledge have?*

**Orient** — Adoption outcome: shared understanding of who owns what. Not a contract.

**Assess** — Playbook-internal step: discover what exists today. User-facing language: *understand your project as it exists today.*

**Discover before you introduce** — Adoption principle: map existing structure before creating new structure. See [ADR-003](../decisions/ADR-003-product-narrative.md).

---

## Validation environments

Evidence model vocabulary — not a framework contract. See [releases/v0.2/evidence.md](../../releases/v0.2/evidence.md).

| Term | Meaning |
|------|---------|
| **Validation environment** | A repository or project context where Anchor evidence is collected. Four types below. |
| **Meta-repo** | Anchor validating itself (`agentic-workflow`). |
| **Validation project (existing)** | An existing mature repository used for maintainer evidence (orient-project Branch B). Any mature repo qualifies—not a product category. Current maintainer instance: `jon-ohio-portfolio`. |
| **Validation project (greenfield)** | A new project started with Anchor from day one (orient-project Branch A). |
| **Independent adopter** | External project outside maintainer control; highest-value evidence for generalization. |

Historical ADRs use *portfolio validation* for validation project (existing).

**Structured log tags** (observations `Source` column only—never use in prose):

| Tag | Environment |
|-----|-------------|
| `meta` | Meta-repo |
| `validation-existing` | Validation project (existing) |
| `greenfield` | Validation project (greenfield) |
| `independent` | Independent adopter |

---

## Contracts

Each term points to its owner — see [Project Entry](../project/entry.md) for definitions.

**Project Entry** · **Specification** · **ADR** · **Skill** · **Playbook** · **Review** · **Handoff**

---

## Milestones

**Foundation** — v0.1 framework structure complete. See [ADR-002](../decisions/ADR-002-framework-vs-experience.md).

**v0.2** — Product narrative shipped. Evidence Window open. See [releases/v0.2](../../releases/v0.2/release.md).

**Release Governance** — How Anchor evolves. See [releases/governance.md](../../releases/governance.md).

**Evidence Window** — After a release ships; contributors record observations; maintainers decide at Evidence Review.
