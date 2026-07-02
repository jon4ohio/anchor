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
| 2 | jon-ohio-portfolio | Existing | Maintainer | Experiment complete (maintainer) | Maintainer validation project (existing); [Context arbitration experiment](context-arbitration-experiment.md) — await independent replication |
| 3 | External #1 | Greenfield (Branch A) | Independent | Pending | |
| 4 | External #2 | Existing (Branch B) | Independent | Pending | |

---

## Observations log

| Date | Source | Type | Observation |
|------|--------|------|-------------|
| 2026-06-30 | meta-repo | friction | README was framework-first before v0.2 — resolved by product page |
| 2026-06-30 | meta-repo | friction | start-project implied greenfield only — resolved by orient-project |
| 2026-06-30 | validation-existing | friction | 74+ ADRs may intimidate newcomers — observe if repeated twice |
| 2026-06-30 | maintainer | hypothesis | Adopters may experience onboarding friction because README and Ch. 4 require navigation through documentation structure before making project-type decisions |
| 2026-06-30 | maintainer | hypothesis | An outcome-first Ch. 4 opening + conversational README Get started may reduce decision latency before adopters begin orienting their project |
| 2026-06-30 | maintainer | hypothesis | Phase 2 Ch. 4 rewrite + cross-links shipped pending independent adopter behavioral signals |
| 2026-06-30 | maintainer | friction | Maintainer-adopter: "What to paste?", "How to start new AI session?", "Explain Anchor every time?", "Should AI read Entry first?" — Ch. 4 did not surface Entry §4 contributor model for AI |
| 2026-06-30 | maintainer | hypothesis | Lightweight AI orientation guidance may reduce context reconstruction at the start of new AI sessions. The appropriate implementation remains unknown and may change as AI tooling evolves |
| 2026-06-30 | maintainer | friction | Moment 2: "How do I ask my AI/collaborator to adopt Anchor correctly?" — distinct from ongoing session orientation (Working with AI) |
| 2026-06-30 | maintainer | hypothesis | Delegating adoption guidance in Ch. 4 may reduce adoption delegation friction without duplicating playbook steps or creating official prompts |
| 2026-07-01 | validation-existing | friction | AI on jon-ohio-portfolio ignored stale Handoff; reconstructed from git/ADRs — unconstrained context gatherer |
| 2026-07-01 | maintainer | hypothesis | Context arbitration: delegated responsibility resolution may produce minimum sufficient context per session |
| 2026-07-01 | maintainer | hypothesis | Four-layer Responsibilities model — ontology only until sub-test shows predictive value vs protocol-only |
| 2026-07-01 | validation-existing | confidence | Maintainer Sessions 0–5 on jon-ohio-portfolio: treatment bundles avg 1.5 files vs baseline 8; negative control passed; stop condition not fired — [experiment log](context-arbitration-experiment.md) |
| 2026-07-02 | maintainer | landscape | Evaluated OpenWiki (AI-oriented repo documentation). Improves implementation representation, not responsibility arbitration. Vendor-independent class: generated implementation docs. |
| 2026-07-02 | maintainer | hypothesis | Unknown whether richer implementation documentation changes the value or operation of context arbitration. Plausible outcomes include no change, increased value, reduced value, or task-class differentiation. Requires empirical use rather than landscape analysis. |
| 2026-07-02 | maintainer | hypothesis | When generated implementation docs conflict with contracts, canonical owner should be the contract for that responsibility (ADR for rationale, Spec for scope, Entry for identity). Untested in practice. |
| 2026-07-02 | maintainer | confidence | Governance process functioned: external tool evaluated → classified → intentionally not promoted → remains observation. Methodological evidence, not capability evidence. |
| 2026-07-02 | maintainer | hypothesis | Recurring theme across context arbitration, adoption teaching, and generated-docs tools: which knowledge should influence this decision right now? — label TBD; watch for independent repetition. |
| 2026-07-02 | maintainer | confidence | anchor-lab Experiment 001 instrument v0.2 — score-first results narrative, responsibility-only animation, opt-in Anchor mapping disclosure. Tests classification prerequisite only; synthesis in [anchor-lab](https://github.com/jon4ohio/anchor-lab) before Anchor protocol citations. |
| 2026-07-02 | maintainer | confidence | anchor-lab Experiment 001 instrument deployed (Tasklight MCQ lesson, GitHub Pages). Tests experiential adoption hypothesis; independent recruitment pending — synthesis in [anchor-lab](https://github.com/jon4ohio/anchor-lab) before Anchor protocol citations. |
| 2026-07-02 | maintainer | confidence | Meta-repo dogfoods thin `AGENTS.md` as one implementation of discoverable AI dispatch (not a framework contract). Capability ≠ filename; Entry remains canonical. Adopting-project concern. |
| 2026-07-02 | maintainer | hypothesis | Discoverable AI starting points may reduce session-start friction for tool-using collaborators. `AGENTS.md` is a common implementation today—not a framework requirement. |

---

## Landscape observations

*This subsection records current explanatory models derived from landscape observations. It is not normative framework guidance and may be revised or removed during Evidence Review.*

**Retrieval pipeline (explanatory model only):** implementation representation (OpenWiki, IDE index, code graph) → retrieval → responsibility classification → context arbitration → reasoning. Anchor's contribution is concentrated in responsibility classification and context arbitration — upstream of retrieval, not documentation generation.

**Non-actions from this landscape review:** no OpenWiki integration; no new position paper; no Entry/ADR/Experience changes; no roadmap items for documentation generators; no promotion of "knowledge arbitration layer" to framework identity.

**Disconfirming evidence welcome:** if generated implementation docs make context arbitration unnecessary for most routine tasks, that narrows Anchor's scope — a valid finding, not a process failure.

---

## AGENTS.md observation watch (meta-repo)

*Watch questions for the meta-repo AI entry point (`AGENTS.md` today). Not normative guidance. Revise or remove at Evidence Review.*

**Hypothesis (2026-07-02):** Discoverable AI starting points may reduce session-start friction for tool-using collaborators. Current implementation: `AGENTS.md`. Questions below are tool- and filename-neutral where possible.

| Question | Positive signal | Negative signal |
| -------- | --------------- | --------------- |
| Do contributors naturally begin from the repository's AI entry point? | Entry point used | Ignored |
| Does it reduce orientation mistakes (wrong owner, missing Handoff)? | Less friction | No measurable change |
| Do contributors try to duplicate canonical contracts into the entry point? | Drift detected | Dispatch remains thin |
| Does the entry point remain stable across releases? | Thin dispatch | Gradual wiki creep |
| Do independent adopters converge on a similar dispatch pattern? | Pattern generalizes | Pattern remains meta-repo specific |

Repeated duplication into the entry point is the signal that would justify codifying a removal test later—not before evidence.

Log findings in **Observations log** above (`friction`, `confidence`, or `hypothesis` as appropriate). No synthetic probes—normal meta-repo, validation environment, or adopter work only.

**Disconfirming evidence welcome:** if the entry point is unused and friction unchanged, that narrows the capability hypothesis—valid finding.

---

## Evidence chain

Anchor's broader claim spans multiple instruments. Each link is tested separately — no single experiment proves the full thesis.

```text
Classify by responsibility     ← anchor-lab Experiment 001 (recruitment open)
        ↓
Organize repos consistently    ← orient-project adoption (not instrumented)
        ↓
AI retrieves correct knowledge ← context arbitration (maintainer complete)
        ↓
Context reconstruction decreases ← jon-ohio-portfolio observational phase
        ↓
Project continuity improves  ← independent adopters (pending)
```

**Experiment 001 (2026-07-02, instrument v0.2):** Tests only the first link — whether responsibility-first classification is learnable experientially. Post-measurement narrative contextualizes results; contract mapping is opt-in disclosure. Full protocol: [anchor-lab experiment-001](https://github.com/jon4ohio/anchor-lab/blob/main/research/experiment-001.md). Validation environment taxonomy: [Glossary — Validation environments](../../docs/experience/glossary.md#validation-environments).

**Context arbitration:** Tests retrieval layer (link 3). See below.

---

## Context arbitration experiment

**Research question:** Can Anchor reliably determine the minimum sufficient context for a session?

**Governing principle:** The adapter is the instrument, not the intervention.

**Full protocol:** [context-arbitration-experiment.md](context-arbitration-experiment.md) — predictions, stop condition, threats to validity, failure attribution, session log.

**Position paper (draft, pending review):** [POSITION-context-arbitration.md](../../docs/decisions/POSITION-context-arbitration.md)

**Label:** Maintainer experiment on `jon-ohio-portfolio` in Cursor — not independent evidence.

**Result (2026-07-01):** Preliminary positive signal. Pass threshold met for feasibility. See [session log and conclusion](context-arbitration-experiment.md#conclusion).

**Capability vs identity:** Experiment supports minimum sufficient context as a **capability** on one project. Does **not** support Anchor identity as responsibility-coordination framework until independent adopter replication.

**Phase:** Controlled complete → [observational phase](context-arbitration-experiment.md#observational-phase) open. Highest-value next evidence: independent adopter (not more maintainer probes).

---

## Validation project (existing) — maintainer hypothesis

**Repository:** `jon-ohio-portfolio` — maintainer validation project (existing).  
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

- `jon-ohio-portfolio` already uses Anchor contracts. orient-project Branch B confirms mapping — no eighth contract needed.
- `AGENTS.md` is not a Skill — boundary matches CONTRIBUTING exclusions.
- Journey Session 2 CLAUDE.md example applies to bloated AI context; this repo uses thin `AGENTS.md` + Entry — variant path.

### Continue — observation

Overlay adoption validates: mature ADR tree + Entry + Handoff without restructuring.

Context arbitration maintainer experiment (2026-07-01): session adapter + falsification Sessions 0–5 complete. Preliminary positive signal — see [experiment log](../releases/v0.2/context-arbitration-experiment.md).

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
- [x] Existing validation project hypothesis documented
- [ ] Independent adopter — greenfield (Branch A)
- [ ] Independent adopter — existing project (Branch B)
- [ ] Evidence Review completed
- [ ] [decision.md](decision.md) filed with Next State
