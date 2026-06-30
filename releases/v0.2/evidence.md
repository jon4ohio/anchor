# Evidence — v0.2

Record observations from applying [orient-project](../../ai/playbooks/orient-project.md). Do not answer from theory.

**Governance:** [governance.md](../governance.md)

---

## Friction questions

- What confused you?
- What felt unnecessary?
- What did you expect that didn't happen?
- What did you understand without explanation?

---

## Confidence questions

- What did you trust without needing to verify?
- When did you stop feeling like you had to reconstruct the project?
- Was there a moment you could simply continue?

---

## Environments

| # | Repository | Branch | Adopter | Status | Notes |
|---|------------|--------|---------|--------|-------|
| 1 | Anchor meta-repo | Existing | Maintainer | Complete | Self-review; [Handoff](../../ai/handoff.md) 2026-06-30 |
| 2 | jon-ohio-portfolio | Existing | Maintainer | Hypothesis | [Portfolio worksheet](#portfolio-existing-project) — not independent evidence |
| 3 | External #1 | Greenfield (Branch A) | Independent | Pending | |
| 4 | External #2 | Existing (Branch B) | Independent | Pending | |

---

## Observations log

| Date | Source | Type | Observation |
|------|--------|------|-------------|
| 2026-06-30 | meta-repo | friction | README was framework-first before v0.2 — resolved by product page |
| 2026-06-30 | meta-repo | friction | start-project implied greenfield only — resolved by orient-project |
| 2026-06-30 | portfolio (hypothesis) | friction | 74+ ADRs may intimidate newcomers — observe if repeated twice |
| 2026-06-30 | maintainer | hypothesis | Adopters may experience onboarding friction because README and Ch. 4 require navigation through documentation structure before making project-type decisions |
| 2026-06-30 | maintainer | hypothesis | An outcome-first Ch. 4 opening + conversational README Get started may reduce decision latency before adopters begin orienting their project |
| 2026-06-30 | maintainer | hypothesis | Phase 2 Ch. 4 rewrite + cross-links shipped pending independent adopter behavioral signals |
| 2026-06-30 | maintainer | friction | Maintainer-adopter: "What to paste?", "How to start new AI session?", "Explain Anchor every time?", "Should AI read Entry first?" — Ch. 4 did not surface Entry §4 contributor model for AI |
| 2026-06-30 | maintainer | hypothesis | Lightweight AI orientation guidance may reduce context reconstruction at the start of new AI sessions. The appropriate implementation remains unknown and may change as AI tooling evolves |
| 2026-06-30 | maintainer | friction | Moment 2: "How do I ask my AI/collaborator to adopt Anchor correctly?" — distinct from ongoing session orientation (Working with AI) |
| 2026-06-30 | maintainer | hypothesis | Delegating adoption guidance in Ch. 4 may reduce adoption delegation friction without duplicating playbook steps or creating official prompts |

---

## Portfolio (existing project) — maintainer hypothesis

**Repository:** `jon-ohio-portfolio`  
**Method:** orient-project Branch B — assess and classify only (no migration).

**Not independent evidence** — framework author assessment. Await independent adopter confirmation.

### Assess — artifacts coordinating the project

| Artifact | Role today |
|----------|------------|
| `README.md` | Dev setup + pointer to Entry and Handoff |
| `docs/project/entry.md` | Project identity and contract index |
| `docs/adrs/` (74+ ADRs) | Decision history |
| `ai/handoff.md` | Session continuity |
| `AGENTS.md` | Next.js agent rules (tooling-specific) |
| `docs/theme-tokens.md`, `docs/figma-*.md` | Reference / implementation guides |

### Classify — responsibility mapping

| Artifact | Responsibility | Anchor contract | Action |
|----------|----------------|-----------------|--------|
| `docs/project/entry.md` | Project identity | Entry | Keep — already aligned |
| `docs/adrs/ADR-*.md` | Decisions | ADR | Keep — strong ADR discipline |
| `ai/handoff.md` | Session continuity | Handoff | Keep |
| `README.md` | Visitor + dev onboarding | Product page / pointer to Entry | Keep split |
| `AGENTS.md` | Tool operating rules | Adopting-project | Keep outside framework |
| Case study pages in `app/work/` | Intended behavior / narrative | Spec-like (per case study) | Project-specific |

### Orient — gaps

- Portfolio already uses Anchor contracts. orient-project Branch B confirms mapping — no eighth contract needed.
- `AGENTS.md` is not a Skill — boundary matches CONTRIBUTING exclusions.
- Journey Session 2 CLAUDE.md example applies to bloated AI context; portfolio uses thin `AGENTS.md` + Entry — variant path.

### Continue — observation

Overlay adoption validates: mature ADR tree + Entry + Handoff without restructuring.

---

## Per-environment worksheet

### Assess

What artifacts coordinated the project before Anchor?

### Classify

| Artifact | Responsibility | Mapped contract |
|----------|----------------|-----------------|
| | | |

### Orient

What gaps were filled? What was kept unchanged?

### Continue

After one work session, was reconstruction avoided?

---

## Evidence Window exit checklist

- [x] Maintainer self-review (meta-repo)
- [x] Portfolio hypothesis documented
- [ ] Independent adopter — greenfield (Branch A)
- [ ] Independent adopter — existing project (Branch B)
- [ ] Evidence Review completed
- [ ] [decision.md](decision.md) filed with Next State
