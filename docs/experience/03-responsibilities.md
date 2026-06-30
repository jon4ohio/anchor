# Responsibilities

Anchor organizes project knowledge by **responsibility**, not by filename.

Ask one question repeatedly:

> **What responsibility does this knowledge have?**

Then map the answer to a contract owner. You do not memorize seven contracts — you recognize which job the knowledge is doing.

---

## Responsibility → contract

| Responsibility | Contract | Question it answers |
|----------------|----------|---------------------|
| Project identity | Entry | What is this project? |
| Decision | ADR | Why did we decide this? |
| Intended behavior | Spec | What are we building? |
| Expertise | Skill | How do we do this kind of work well? |
| Quality | Review | Is this good enough? |
| Procedure | Playbook | What order do we do things in? |
| Session continuity | Handoff | What changed recently? |

Knowledge has responsibilities. Contracts formalize responsibilities.

---

## Example: `CLAUDE.md` doing three jobs

John's Session 1 `CLAUDE.md` mixed:

| Content | Responsibility | Belongs in |
|---------|----------------|------------|
| "tasklight is a CLI…" | Project identity | Entry |
| "Always run tests before commit" | Operating instruction | `CLAUDE.md` (trimmed) |
| "We're working on export next" | Session continuity | Handoff |
| "Why SQLite: single file…" | Decision | ADR-001 (already exists) |

Anchor does not delete `CLAUDE.md`. It separates responsibilities so the file stops competing with durable owners.

The same analysis applies to `AGENTS.md`, `GEMINI.md`, copilot instructions, and architecture docs that mix decision rationale with layout description.

---

## Files may not move

Orientation maps ownership. Migration is optional. John's ADR stayed in `docs/decisions/`. Only missing contracts were created (Entry, Spec, Handoff).

See [Session 2 snapshot](../../journey/john-ohio/sessions/02-separate/SESSION.md).

---

## Next

[Chapter 4 — Adopt Anchor](04-building-your-own.md)
