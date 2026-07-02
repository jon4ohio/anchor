# SPEC-001: Knowledge Structure

**Contract:** Specification  
**Status:** Active  
**Problem coordinated:** How should collaborative knowledge be structured?

---

## Promise

Define what we are building: a coordination framework for structuring collaborative knowledge in software projects.

---

## Problem

Repositories store code, READMEs, docs, ADRs, issues, and PRs—but these describe pieces of a project, not the project itself. Humans and AI repeatedly reconstruct the same mental model through conversation.

Important information fragments across channels. The result:

- Repeated explanations of the same decisions
- Inconsistent assumptions between collaborators
- AI hallucinating project intent from incomplete context
- One-off prompts reinvented every session

We need a structure that coordinates understanding, decisions, scope, expertise, execution, quality, and continuity—without becoming a wiki.

---

## Goals

1. Enable any contributor (human or AI) to understand and contribute without rediscovering context.
2. Define exactly seven contracts, each owning one kind of truth.
3. Keep the framework lean enough to dogfood on itself and portable across projects.
4. Validate through usage on three projects before evolving to v0.2.

---

## Requirements

### Framework structure

- [x] Seven contracts defined: Project Entry, Specification, ADR, Skill, Playbook, Review, Handoff
- [x] Four principles enforced: contracts not files; one owner per truth; reference don't duplicate; promote only after repetition
- [x] Collaboration lifecycle documented: Understand → Decide → Execute → Review → Improve
- [x] Each contract has Promise, Owns, Must never contain, and Lifecycle

### Repository bootstrap

- [x] All seven contracts represented as files in this repository
- [x] Each file names the problem it coordinates
- [x] Project Entry indexes all operative contracts
- [x] Zero duplication of owned content across contracts
- [x] Git initialized; repository is tool-agnostic markdown

### Usability

- [x] A cold-start contributor can read Entry → this Spec → Handoff without prior chat context
- [x] Playbook exists for bootstrapping new projects
- [x] Review checklist exists for contract ownership

---

## Acceptance Criteria

1. A new collaborator orients via [Project Entry](../project/entry.md) in under five minutes.
2. All seven contracts exist and pass the [contract-ownership Review](../../ai/reviews/contract-ownership.md).
3. No contract restates content owned by another contract.
4. Handoff records validation horizon (validation project (existing), greenfield) and open empirical questions.
5. Skill is marked experimental; no canonical Skill template is implied.

---

## Out of Scope

- Markdown templates or folder structure mandates for other projects
- YAML schemas, frontmatter requirements, or automated conformance
- Existing-project and greenfield validation (planned, not part of this spec's delivery)
- Eighth contract types
- Resolving Skill definition (deferred to validation project (existing))

---

## Edge Cases

| Situation | Handling |
|---|---|
| Content fits two contracts | Apply one owner per truth; reference the owner |
| Useful idea mentioned once | Handoff or conversation; do not promote |
| Decision reverses a prior decision | Supersede ADR; do not mutate original |
| Entry needs to mention a decision | One-line pointer to ADR; no rationale in Entry |

---

## Related ADRs

- [ADR-001: Artifacts Became Contracts](../decisions/ADR-001-contracts-not-artifacts.md)

---

## Technical Notes

Implementation is markdown in version control. Contract type is identifiable by location and document heading. No build step, no tooling dependency.

Layout in this repository is one implementation, not the framework itself. Other projects may organize files differently if contracts and ownership rules are preserved.
