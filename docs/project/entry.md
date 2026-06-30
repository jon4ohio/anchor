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

Version-controlled coordination for collaborative software projects.

## 1. Purpose

**Anchor is intentionally small. Expand the framework only when repeated evidence across independent projects shows the existing contracts are insufficient.**

**Anchor is a coordination framework for durable project context.** It helps humans and AI work from the same shared understanding by coordinating orientation, decisions, implementation scope, expertise, execution, quality, and continuity.

**Adopting projects:** Assess existing structure before introducing new structure. Knowledge has responsibilities; contracts formalize those responsibilities. Existing ADRs, documentation, and AI context files may already serve contract roles—orientation maps ownership before creating new artifacts. See [ADR-003](../decisions/ADR-003-product-narrative.md) and [orient-project Playbook](../../ai/playbooks/orient-project.md).

In the lifecycle below, **Execute** means Spec + Playbook phase ordering—not how adopting projects run tools or agents.

Anchor is not a documentation convention, an AI prompt library, or a wiki. It is a set of **contracts**—reliable promises about what each piece of project knowledge owns and how collaborators should use it.

This repository uses Anchor to build Anchor. Every contract here exists because a real coordination problem demanded it.

---

## 2. Principles

### Four enduring principles

1. **Contracts, not files.** A markdown file is one implementation of a promise. The contract is the promise itself.

2. **One owner per truth.** Each contract owns exactly one kind of truth. No two contracts may assert the same thing.

3. **Reference, don't duplicate.** When another contract owns a truth, link to it. Never restate it.

4. **Promote only after repetition.** One useful conversation is not a Skill. One checklist is not a Review. One workflow is not a Playbook. Only when something recurs should it become a contract. **Framework evolution** requires repeated evidence across independent projects—not anticipation from the meta-repo alone.

### Seven contracts

| Contract | Coordinates | Question answered |
|---|---|---|
| Project Entry | Orientation | What is this project? |
| Specification | Implementation scope | What are we building? |
| ADR | Decisions | Why did we decide this? |
| Skill | Transferable coordination expertise | How do we perform this kind of work well across projects? |
| Playbook | Execution | How do we run this workflow? |
| Review | Quality | Is this good enough? |
| Handoff | Continuity | What changed recently? |

No eighth contract without proven repetition across real projects.

**Skill hypothesis (v0.1):** A Skill captures transferable expertise that improves coordination across projects. The current exemplar is [what-to-keep.md](../../ai/skills/what-to-keep.md). Adoption validation confirms or refines.

---

## 3. Contract Definitions

Each contract follows the same schema: Promise, Owns, Must never contain, Lifecycle.

### Project Entry

**Promise:** Orient a contributor in under five minutes—including where durable truths live.

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

**Promise:** Teach transferable expertise that improves coordination across projects.

**Owns:** Principles, rules, examples for judgment, heuristics, or reasoning patterns—not tool dispatch.

**Must never contain:** Project-specific requirements (Specs), sequential workflows (Playbooks), pass/fail checklists (Reviews), tool invocation, agent routing, or prescribing how adopting projects organize their work.

**Lifecycle:** Reusable across projects. Refined continuously after repetition proves value.

**Implementation in this repo:** [what-to-keep.md](../../ai/skills/what-to-keep.md) — current exemplar, not the definition of all future Skills.

---

### Playbook

**Promise:** Prescribe execution order for a recurring activity.

**Owns:** Sequential steps and which contracts to read or update at each step.

**Must never contain:** Expertise teaching (reference Skills), quality criteria (reference Reviews), requirements (reference Specs).

**Lifecycle:** Created after a workflow repeats. Updated when the workflow changes.

**Implementation in this repo:** [orient-project.md](../../ai/playbooks/orient-project.md) (adoption); [start-project.md](../../ai/playbooks/start-project.md) (redirect)

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

**Owns:** Session truth—delta (what changed), horizon (what is active), blocks, session questions, current branch/PR pointers, friction.

**Must never contain:** Project truth that has graduated (settled decisions → ADR, requirements → Spec, evaluation criteria → Review).

**Lifecycle:** Rolling document. Conversation → Handoff → contract or discarded. Anything unchanged after three cycles graduates to another contract or is deleted.

**Implementation in this repo:** [handoff.md](../../ai/handoff.md)

---

## 4. Protocol

Every contributor—human or AI—follows the same lifecycle:

```
Understand → Decide → Execute → Review → Improve
```

| Phase | Contract | Action |
|---|---|---|
| Understand | Project Entry | Read this document. Orient to the project and where durable truths live. |
| Understand | — | Consult any project-specific implementation guidance before beginning implementation work, if the adopting project provides it. |
| Decide | ADR | Record decisions that constrain future work. |
| Execute | Spec + Playbook | Define scope; follow execution order. |
| Review | Review | Run applicable checklists. |
| Improve | Handoff | Record delta and horizon for the next session. |

**Skills sit beside the lifecycle.** They are reusable capability, not project state. Playbooks reference Skills; they do not embed them.

Not every phase applies to every task. Use judgment. Create an ADR only when a decision constrains future work—not for every implementation choice.

---

## 5. Governance

### Scope

Anchor preserves durable project context. It does not prescribe project execution.

Future framework additions must preserve durable project context. How adopting projects organize tooling, workflows, and agents is outside Anchor.

### Two products

Anchor has two products:

- **Framework** — seven contracts (this document). Defines the system.
- **Experience** — adoption documentation at [docs/experience/](../../docs/experience/). Teaches the system.
- **Operations** — repeatable procedures in [Playbooks](../../ai/playbooks/) (start, validate, publish). Executes the system.

Framework documents define the system. Experience documents teach the system. Operations playbooks execute the system. Experience structure may exist early; **content** expands only after the same adoption question appears twice in validation. See [ADR-002](../decisions/ADR-002-framework-vs-experience.md).

### User language

The framework should use the language its users already think in—not the framework author's jargon.

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
| Same tool or agent dispatch question | Adopting project documentation |
| Same workflow twice | Playbook |
| Same quality gate twice | Review |

### Experience expansion

| Signal | Action |
|---|---|
| Same adoption question twice in validation | Expand relevant Experience guide |
| New term enters common use | Update [Experience glossary](../../docs/experience/glossary.md) |

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

**Foundation Complete → Validation → Release → Evolution**

1. **This repo** — Anchor dogfoods itself; foundation milestone complete
2. **Adoption validation** — first adopter (natural work; friction log); follow [Validate Through Use Playbook](../../ai/playbooks/validate-through-use.md)
3. **Greenfield project** — day-one start via [Orient Project Playbook](../../ai/playbooks/orient-project.md) Branch A

When you need to explain something, pause and ask: *Which contract owns this?*

Success: after three uses, the same seven contracts and four principles hold without an eighth. No framework changes without evidence from at least two independent projects.

---

## Contract Index

| Contract | Location |
|---|---|
| Project Entry | [entry.md](entry.md) (this file) |
| Specification | [SPEC-001](../specs/SPEC-001-knowledge-structure.md) |
| ADR | [ADR-001](../decisions/ADR-001-contracts-not-artifacts.md) |
| Skill | [what-to-keep.md](../../ai/skills/what-to-keep.md) |
| Playbook | [orient-project.md](../../ai/playbooks/orient-project.md) |
| Review | [contract-ownership.md](../../ai/reviews/contract-ownership.md) |
| Handoff | [handoff.md](../../ai/handoff.md) |

**Experience (product documentation, not contracts):** [docs/experience/](../../docs/experience/)

---

## Glossary

| Term | Meaning |
|---|---|
| Contract | A promise about what truth an artifact owns and how to use it |
| Coordinate | To align collaborators around a specific kind of work without ambiguity |
| Promote | To elevate repeated informal knowledge into a contract |
| Supersede | To replace an ADR with a newer ADR; the old record stays immutable |
| Dogfood | To use Anchor on the project that defines Anchor |
