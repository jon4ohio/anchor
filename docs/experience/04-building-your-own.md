# Building Your Own Anchor

Adopt Anchor incrementally. Keep what works. Orient what exists. Fill gaps only where coordination is missing.

Follow the [Orient Project playbook](../../ai/playbooks/orient-project.md).

---

## How are you adopting Anchor?

### New project {#new-project}

You have little to discover. Orientation establishes initial contracts:

1. Assess — empty or minimal repo; identify first real work
2. Classify — which responsibilities will you need first? (usually Entry + first Spec)
3. Orient — create missing owners; point README to Entry
4. Continue — normal work; Handoff between sessions

See [Orient Project — Branch A](../../ai/playbooks/orient-project.md#branch-a-new-project).

### Existing project {#existing-project}

You have ADRs, docs, AI context files, maybe team conventions. Orientation discovers before introducing:

1. Assess — list artifacts that coordinate the project today
2. Classify — what responsibility does each serve?
3. Orient — map to contracts; trim overlap (especially in AI context files)
4. Fill gaps only — create contracts only where no owner exists
5. Continue — normal work

See [Orient Project — Branch B](../../ai/playbooks/orient-project.md#branch-b-existing-project).

---

## I already have…

| I already have… | Anchor says… |
|-----------------|--------------|
| ADRs | Keep them. Map to Decision responsibility. |
| `CLAUDE.md` / AI context | Keep them. Narrow to operating instructions; point durable truth to owners. |
| Architecture docs | Keep them. Clarify whether they own layout (reference) or decisions (ADR). |
| Good README | Keep it. Product page for visitors; Entry for contributors. |
| Random notes | Classify — Handoff, Spec, or discard. |

---

## After orientation

- Update Handoff each session
- Promote repeated explanations per [what-to-keep Skill](../../ai/skills/what-to-keep.md)
- Run [contract-ownership Review](../../ai/reviews/contract-ownership.md) when adding contracts

---

## Next

[Chapter 5 — Framework Reference](05-framework-reference.md) when you need contract precision.

[Canonical Journey](../../journey/john-ohio/README.md) for a full walkthrough.
