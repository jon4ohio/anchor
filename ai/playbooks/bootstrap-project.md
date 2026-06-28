# Playbook: Bootstrap a Project with Anchor

**Contract:** Playbook  
**Problem coordinated:** How do we bootstrap a new project with Anchor?

---

## Promise

Prescribe execution order for initializing Anchor on a new or existing repository.

---

## Prerequisites

- Empty or existing git repository
- Decision to validate Anchor through usage, not further design

---

## Steps

### 1. Understand — Project Entry

Create the Project Entry contract. Include: purpose, four principles, seven contracts overview, protocol, governance, contract index.

If README exists, keep it minimal—a pointer to Entry, not a duplicate.

### 2. Decide — ADR

Record the first significant decision as an ADR if one exists (e.g., why Anchor, why these contracts). Skip if no decision constrains future work yet.

See [ADR format](../../docs/decisions/ADR-001-contracts-not-artifacts.md) in this repo as one implementation.

### 3. Execute — Specification

Write a Spec for the first real work the project demands. Name the problem it coordinates. Define requirements and acceptance criteria. Reference ADRs; do not restate rationale.

### 4. Execute — Playbook and Skill (if repetition warrants)

Create Playbooks only after a workflow repeats. Create Skills only after expertise questions recur across sessions or projects.

For the first project, bootstrap Playbook (this file) and an experimental Skill probe may exist from the meta-repo.

Reference: [distillation Skill](../skills/distillation.md)

### 5. Review — Run ownership checklist

Run [contract-ownership Review](../reviews/contract-ownership.md) against all contract files. Fix violations before proceeding.

### 6. Improve — Handoff

Write or update [Handoff](../handoff.md). Record delta, horizon, blocks, and session questions. Note open empirical questions for v0.2.

---

## After Bootstrap

Apply the post-project review question after each project:

> What repeated coordination problem wasn't handled cleanly by the existing contracts?

Record answers in Handoff or friction log.

---

## References

- [Project Entry](../../docs/project/entry.md)
- [distillation Skill](../skills/distillation.md)
- [contract-ownership Review](../reviews/contract-ownership.md)
