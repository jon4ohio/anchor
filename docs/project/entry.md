# Project Entry

**Contract:** Project Entry  
**Problem coordinated:** Where am I? What is this project?

---

## Promise

Orient a new contributor in under five minutes.

---

## Owns

- Project identity and purpose
- Coordination framework definition (this document)
- Four principles and seven contracts
- Collaboration protocol and governance rules
- Index of all operative contracts in this repository

---

## Must Never Contain

- Decision rationale (see [ADR-001](../decisions/ADR-001-contracts-not-artifacts.md))
- Feature requirements (see [SPEC-001](../specs/SPEC-001-knowledge-structure.md))
- Sequential workflows (see [Playbooks](../../ai/playbooks/))
- Quality checklists (see [Reviews](../../ai/reviews/))
- Session state or recent deltas (see [Handoff](../../ai/handoff.md))

Entry is the only composite contract. It aggregates pointers and project-level framing—it does not aggregate content owned elsewhere.

---

# Anchor v0.1

## 1. Purpose

**Anchor is a coordination framework.** It helps humans and AI work from the same shared understanding by coordinating orientation, decisions, implementation scope, expertise, execution, quality, and continuity.

Anchor is not a documentation convention, an AI prompt library, or a wiki. It is a set of **contracts**—reliable promises about what each piece of project knowledge owns and how collaborators should use it.

This repository uses Anchor to build Anchor. Every contract here exists because a real coordination problem demanded it.

---

## 2. Principles

### Four enduring principles

1. **Contracts, not files.** A markdown file is one implementation of a promise. The contract is the promise itself.

2. **One owner per truth.** Each contract owns exactly one kind of truth. No two contracts may assert the same thing.

3. **Reference, don't duplicate.** When another contract owns a truth, link to it. Never restate it.

4. **Promote only after repetition.** One useful conversation is not a Skill. One checklist is not a Review. One workflow is not a Playbook. Only when something recurs should it become a contract.

### Seven contracts

| Contract | Coordinates | Question answered |
|---|---|---|
| Project Entry | Orientation | What is this project? |
| Specification | Implementation scope | What are we building? |
| ADR | Decisions | Why did we decide this? |
| Skill | Expertise | How do we perform this kind of work? |
| Playbook | Execution | How do we run this workflow? |
| Review | Quality | Is this good enough? |
| Handoff | Continuity | What changed recently? |

No eighth contract without proven repetition across real projects.

**Skill is experimental in v0.1.** The contract slot exists; its precise definition is deliberately unresolved. Usage on multiple projects will reveal whether a Skill is a methodology, reusable expertise, or something else.

---

## 3. Contract Definitions

Each contract follows the same schema: Promise, Owns, Must never contain, Lifecycle.

### Project Entry

**Promise:** Orient a contributor in under five minutes.

**Owns:** Identity, strategic frame, non-goals, glossary, contract index.

**Must never contain:** Decision rationale, requirements, checklists, session state.

**Lifecycle:** Created early. Updated occasionally when strategic frame changes.

**Composite exception:** Entry is the only contract that aggregates pointers to other contracts.

---

### Specification

**Promise:** Define what we are building for a bounded scope.

**Owns:** Problem statement, goals, requirements, acceptance criteria, edge cases, out-of-scope.

**Must never contain:** Decision rationale (reference ADRs), execution steps (reference Playbooks), quality gates (reference Reviews).

**Lifecycle:** Created per feature or initiative. Updated until complete. May be marked Active, Complete, or Superseded.

**Implementation in this repo:** [SPEC-001](../specs/SPEC-001-knowledge-structure.md)

---

### ADR (Architecture Decision Record)

**Promise:** Explain why a significant decision was made.

**Owns:** Context, decision, alternatives considered, consequences.

**Must never contain:** Task status, roadmap, implementation details better suited to Specs, reusable methodology (reference Skills).

**Lifecycle:** Immutable once accepted. Changed only by supersession with a new ADR.

**Implementation in this repo:** [ADR-001](../decisions/ADR-001-contracts-not-artifacts.md)

---

### Skill *(experimental)*

**Promise:** Teach repeatable expertise for a class of work.

**Owns:** Principles, rules, examples for a transferable capability.

**Must never contain:** Project-specific requirements (Specs), sequential workflows (Playbooks), pass/fail checklists (Reviews).

**Lifecycle:** Reusable across projects. Refined continuously after repetition proves value.

**Open question (v0.1):** What exactly is a Skill? Methodology, expertise body, or something else? Deferred until portfolio validation.

**Implementation in this repo:** [distillation.md](../../ai/skills/distillation.md) — minimal probe, not a canonical template.

---

### Playbook

**Promise:** Prescribe execution order for a recurring activity.

**Owns:** Sequential steps and which contracts to read or update at each step.

**Must never contain:** Expertise teaching (reference Skills), quality criteria (reference Reviews), requirements (reference Specs).

**Lifecycle:** Created after a workflow repeats. Updated when the workflow changes.

**Implementation in this repo:** [bootstrap-project.md](../../ai/playbooks/bootstrap-project.md)

---

### Review

**Promise:** Verify quality without teaching.

**Owns:** Checklist items only. Pass or fail. No explanation.

**Must never contain:** Rationale, principles, examples, sequential steps.

**Lifecycle:** Created after a quality gate repeats. Updated when criteria change.

**Implementation in this repo:** [contract-ownership.md](../../ai/reviews/contract-ownership.md)

---

### Handoff

**Promise:** Coordinate continuity between work sessions.

**Owns:** Delta (what changed), horizon (what is active), blocks, session questions, current branch/PR pointers.

**Must never contain:** Settled decisions, requirements, principles, checklists, strategic framing.

**Lifecycle:** Rolling document. Updated whenever meaningful work ends. Anything unchanged after three cycles graduates to another contract or is deleted.

**Implementation in this repo:** [handoff.md](../../ai/handoff.md)

---

## 4. Protocol

Every contributor—human or AI—follows the same lifecycle:

```
Understand → Decide → Execute → Review → Improve
```

| Phase | Contract | Action |
|---|---|---|
| Understand | Project Entry | Read this document. Orient to the project. |
| Decide | ADR | Record decisions that constrain future work. |
| Execute | Spec + Playbook | Define scope; follow execution order. |
| Review | Review | Run applicable checklists. |
| Improve | Handoff | Record delta and horizon for the next session. |

**Skills sit beside the lifecycle.** They are reusable capability, not project state. Playbooks reference Skills; they do not embed them.

Not every phase applies to every task. Use judgment. Create an ADR only when a decision constrains future work—not for every implementation choice.

---

## 5. Governance

### Inclusion test

Before creating or expanding any contract, ask:

> Does this own truth that another contract already owns?

If yes, reference the owner instead. If no, ask:

> Has this problem recurred enough to earn a contract?

If no, leave it in conversation or Handoff.

### Promotion

| Signal | Promote to |
|---|---|
| Same "why" question twice | ADR |
| Same requirements discussion twice | Spec |
| Same expertise question across projects | Skill |
| Same workflow twice | Playbook |
| Same quality gate twice | Review |

### Post-project review question

After every project using Anchor, ask:

> **What repeated coordination problem wasn't handled cleanly by the existing contracts?**

| Answer | Action |
|---|---|
| None | Don't change Anchor |
| Handoffs bloated | Improve Handoff contract |
| Same checklist reinvented | Strengthen Review contract |
| Eighth contract needed | Evolve only if repetition is proven |

### Validation path

1. **This repo** — Anchor dogfoods itself
2. **Portfolio repo** — ADRs proven; Entry and Handoff under maintenance
3. **Greenfield project** — day-one bootstrap; Playbook tested without legacy

Success: after three uses, the same seven contracts and four principles hold without an eighth.

---

## Contract Index

| Contract | Location |
|---|---|
| Project Entry | [entry.md](entry.md) (this file) |
| Specification | [SPEC-001](../specs/SPEC-001-knowledge-structure.md) |
| ADR | [ADR-001](../decisions/ADR-001-contracts-not-artifacts.md) |
| Skill | [distillation.md](../../ai/skills/distillation.md) |
| Playbook | [bootstrap-project.md](../../ai/playbooks/bootstrap-project.md) |
| Review | [contract-ownership.md](../../ai/reviews/contract-ownership.md) |
| Handoff | [handoff.md](../../ai/handoff.md) |

---

## Glossary

| Term | Meaning |
|---|---|
| Contract | A promise about what truth an artifact owns and how to use it |
| Coordinate | To align collaborators around a specific kind of work without ambiguity |
| Promote | To elevate repeated informal knowledge into a contract |
| Supersede | To replace an ADR with a newer ADR; the old record stays immutable |
| Dogfood | To use Anchor on the project that defines Anchor |
