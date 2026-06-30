# John's Journey — Narrative

John Ohio builds **tasklight**, a CLI that stores tasks in a local file. He uses Claude Code daily. After six months he has working code, scattered context, and no time to reorganize everything.

---

## Session 1 — Understand

John lists what already coordinates his project:

| Artifact | What John thinks it does |
|----------|--------------------------|
| `README.md` | Explains the CLI to GitHub visitors |
| `docs/architecture.md` | Describes file layout and storage |
| `docs/decisions/ADR-001-sqlite.md` | Records why he chose SQLite |
| `CLAUDE.md` | Tells AI how to work on the repo |
| Chat history | Where most explanations still live |

John does not delete or move anything. He asks: *What responsibility does each piece serve?*

**Outcome:** He sees overlap — especially in `CLAUDE.md` — but has not separated responsibilities yet.

→ [Session 1 snapshot](sessions/01-understand/)

---

## Session 2 — Separate

John asks the responsibility question for each artifact:

| Responsibility | Owner | John's artifact |
|----------------|-------|-----------------|
| Project identity | Entry | `docs/project/entry.md` (new — indexes the rest) |
| Decision | ADR | `docs/decisions/ADR-001-sqlite.md` (already exists) |
| Intended behavior | Spec | `docs/specs/SPEC-001-export.md` (new — export feature) |
| Session continuity | Handoff | `ai/handoff.md` (new) |

**The CLAUDE.md moment:** John's `CLAUDE.md` mixes project identity ("tasklight is a CLI…"), expertise ("always run tests before commit"), and session notes ("we're working on export next"). One file, three responsibilities.

Anchor does not delete `CLAUDE.md`. John trims it to AI operating instructions and points durable truths to their owners. Decisions stay in ADR-001. Export scope moves to SPEC-001.

**Outcome:** Knowledge has responsibilities. Contracts formalize responsibilities. Files mostly stay where they are.

→ [Session 2 snapshot](sessions/02-separate/)

---

## Session 3 — Fill gaps

John implements export per SPEC-001. Before merging he runs a ownership review checklist. He updates Handoff:

- **Delta:** Export command shipped; SPEC-001 complete.
- **Horizon:** Import feature; no open decision blocks.
- **Blocks:** None.

**Outcome:** Only gaps were filled — Entry, Spec, Handoff. Existing ADR and architecture doc kept their roles.

→ [Session 3 snapshot](sessions/03-fill-gaps/)

---

## Session 4 — Return

John vacations for three weeks. He opens tasklight again.

**Without Anchor** he would scroll chat, grep commits, wonder why SQLite again, and risk reopening a settled debate.

**With Anchor** he reads Handoff (30 seconds), opens ADR-001 when he forgets the storage rationale, reads SPEC-001 for export behavior, and continues on import.

**Outcome:** Continue instead of reconstruct.

→ [Session 4 snapshot](sessions/04-return/)

---

## What John did not do

- Migrate every doc into an `ai/` folder
- Replace ADRs with a new format
- Rewrite six months of architecture notes
- Force a greenfield layout on a mature project

He oriented what existed, separated responsibilities, and filled gaps only where coordination was missing.

[Adopt on your project →](../../docs/experience/04-building-your-own.md)
