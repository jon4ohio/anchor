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

**Contributing Evidence** — [Experience Chapter 6](06-contributing-evidence.md); how adopters share observations to help Anchor evolve.

**Closing the Loop** — The lifecycle completes when observations from real projects improve the framework for future adopters. See [Contributing Evidence](06-contributing-evidence.md).

**Product page** — [README.md](../../README.md); discover and evaluate before adopting.

**Experience** — Adoption documentation in this directory. Not a contract.

**Framework** — Seven contracts defined in [Project Entry](../project/entry.md).

**Practice** — A reusable engineering activity (e.g. project orientation, contributing evidence). Not a contract. Catalog: [docs/practices/](../practices/README.md).

**Audience-specific expression** — The same practice expressed for different audiences: Experience chapters for learning, Playbooks for execution, Reviews for verification, Skills for judgment, Reference Projects for demonstration. See [POSITION-audience-specific-expressions](../decisions/POSITION-audience-specific-expressions.md).

**Reference Project** — Anchor's proving ground: evidence, demonstration, teaching, and validation in one layer. Maintainer-owned projects built using Anchor to validate the framework and provide canonical examples. Index: [journey/README.md](../../journey/README.md). Instances: [Examples](examples.md).

---

## Adoption terms

**Responsibility** — The job a piece of knowledge performs (identity, decision, session state, etc.). Ask: *What responsibility does this knowledge have?*

**Orient** — Adoption outcome: shared understanding of who owns what. Not a contract.

**Assess** — Playbook-internal step: discover what exists today. User-facing language: *understand your project as it exists today.*

**Discover before you introduce** — Adoption principle: map existing structure before creating new structure. See [ADR-003](../decisions/ADR-003-product-narrative.md).

---

## Three loops

Defined in [Contributing Evidence](06-contributing-evidence.md). Each coordinates a distinct cycle.

**Delivery Loop** — Build → Observe → Improve Project. Everyday engineering on your project.

**Evidence Loop** — Observe → Contribute Evidence → Anchor Evolves. How project observations improve the framework.

**Learning Loop** — Reference Projects → Examples → Better Adoption. How teaching artifacts improve paths for future adopters.

---

## Validation environments

Evidence model vocabulary — not a framework contract. See [releases/v0.2/evidence.md](../../releases/v0.2/evidence.md).

**Validation environment** — *Where* evidence comes from.

| Environment | Question it answers |
|-------------|---------------------|
| **Reference Project** | Does teaching match current best practice? |
| **Existing Project** | Does adoption work without migration? |
| **Greenfield Project** | Does day-one orientation work? |
| **Independent Adoption** | Does it generalize without maintainer control? |
| **Meta-repo** | Anchor validating itself (`agentic-workflow`). |

Historical ADRs use *portfolio validation* for validation project (existing). **Validation project (existing)** and **Validation project (greenfield)** remain valid terms for maintainer evidence tracking.

**Structured log tags** (observations `Source` column only—never use in prose):

| Tag | Environment |
|-----|-------------|
| `meta` | Meta-repo |
| `reference` | Reference Project |
| `validation-existing` | Validation project (existing) |
| `greenfield` | Validation project (greenfield) |
| `independent` | Independent adopter |

---

## Evidence source

**Evidence source** — *Who* produced the observation. Orthogonal to validation environment.

| Source | Meaning |
|--------|---------|
| **Maintainer** | Maintainer-controlled environments |
| **Contributor** | Community member, not independent adopter |
| **Independent Adopter** | External project outside maintainer control |

Environment and source combine independently—for example, a Reference Project observation is typically Maintainer-sourced; an Independent Adoption observation is Community-sourced.

---

## Evidence contribution

**Observation Guide** — Optional template at [templates/observation-guide.md](templates/observation-guide.md) for capturing observations. Methodology: [docs/practices/contributing-evidence.md](../practices/contributing-evidence.md).

### Evidence levels

Weight of an observation—not a framework contract.

| Level | Signal |
|-------|--------|
| **L0** | Read documentation |
| **L1** | Created or scaffolded project |
| **L2** | Used Anchor through real sessions |
| **L3** | Completed a milestone with Handoff continuity |
| **L4** | Completed a project |
| **L5** | Recommended specific improvements with examples |

Author self-assessment is **hypothesis** until independently corroborated.

---

## Teaching artifacts

| Artifact | Teaches |
|----------|---------|
| **Canonical Journey** | How one project evolved over time |
| **Reference Project** | Current best practice, live demonstration |
| **Independent Adoption** | Generalization without maintainer involvement |

Instances: [Examples](examples.md).

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
