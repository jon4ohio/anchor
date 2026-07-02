# Canonical Journey — John Ohio

John Ohio has been building **tasklight** — a tiny CLI for personal task lists — for six months with AI assistance. This journey shows how Anchor works on a project that already has docs, decisions, and AI context files.

**Slogan:** Continue instead of reconstruct.

---

## The arc

| Session | Beat |
|---------|------|
| [1 — Understand](sessions/01-understand/) | John assesses what he already has |
| [2 — Separate](sessions/02-separate/) | John classifies responsibilities |
| [3 — Fill gaps](sessions/03-fill-gaps/) | John ships with clear owners |
| [4 — Return](sessions/04-return/) | John comes back after three weeks |

Read the full walkthrough in [NARRATIVE.md](NARRATIVE.md).

---

## Iconic diagram

```text
Without Anchor                    With Anchor

Conversation                      Conversation
Conversation                            │
     │                                  ▼
     ▼                            Durable Context
Start over                              │
                                        ▼
                                   Continue
```

---

## Session 4 payoff

```text
Without Anchor                    With Anchor

• Reads weeks of chat             • Reads Handoff
• Searches commits                • Opens ADR-001
• Forgets why SQLite won          • Continues coding
• Reopens settled debates

reconstruct                       continue instead of reconstruct
```

---

## How to use this journey

- **Newcomers:** Read [NARRATIVE.md](NARRATIVE.md) start to finish.
- **Adopters:** Compare your repo to each session snapshot.
- **Questions:** "How should I structure Handoff?" → Session 3. "When to record a decision?" → Session 2.

[Back to README](../README.md) · [Reference Projects](../README.md) · [Experience guides](../../docs/experience/README.md)
