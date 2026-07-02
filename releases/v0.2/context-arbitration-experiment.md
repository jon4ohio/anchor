# Context Arbitration Experiment — jon-ohio-portfolio

**Status:** Controlled phase complete · Observational phase open  
**Governance:** [governance.md](../governance.md) · [evidence.md](evidence.md)  
**Instrument:** `jon-ohio-portfolio` → `ai/session-arbitration.md` + `.cursor/rules/anchor-session-arbitration.mdc`

Conducted on `jon-ohio-portfolio`, the maintainer's validation project (existing).

**Label:** Maintainer experiment — not independent evidence.

**Evidence supports (capability):** Delegated responsibility resolution can produce smaller, sufficient context bundles vs unconstrained retrieval in one real project (Cursor, maintainer-operated).

**Does not support (identity):** Anchor as a responsibility-coordination framework — requires independent adopter gate.

---

## Research question

> Can Anchor reliably determine the **minimum sufficient context** for a session?

## Governing principle

> **The adapter is the instrument, not the intervention.**

We are testing whether **delegated responsibility resolution** changes AI context-selection behavior. The adapter makes the treatment reproducible.

## Conceptual frame (observation)

Context arbitration — given many possible truths, which truths are relevant now?

## Secondary hypothesis (do not promote)

Four-layer Responsibilities model — test whether explicit responsibility modeling improves coordination vs protocol-only rules. Sub-test optional.

---

## Pre-registered predictions

Recorded **2026-07-01** before Session 1. Do not revise without noting change.

| Prediction | Expected direction |
|------------|-------------------|
| Average context bundle size | Smaller than unconstrained baseline |
| Context precision | Higher than baseline (fewer unnecessary artifacts) |
| Git access on answerable questions | Less frequent when bundle suffices |
| Task success rate | No decrease vs baseline |
| Human clarification requests | Lower |
| Handoff trust (proxy) | Higher on continuity questions |

---

## Stop condition

> If two consecutive sessions require expanding the context bundle beyond the protocol's recommendation to complete routine work, suspend the experiment and record the protocol as insufficient.

On stop: do not patch adapter or protocol during Evidence Window; record failure layer; proceed to Evidence Review with negative result.

---

## Failure attribution model

| Layer | What it is | Failure example |
|-------|------------|-----------------|
| **Responsibility** | Orientation — who owns this question? | Wrong owner (continuity vs decision) |
| **Protocol** | Session rules given correct responsibility | Correct owner, wrong context mapping |
| **Adapter** | Tool execution of protocol | Correct protocol, skipped steps |

---

## Threats to validity

| Threat | Description | Mitigation |
|--------|-------------|------------|
| **Maintainer familiarity** | Author knows repo; bundles may appear smaller | Label maintainer experiment; independent adopter before identity change |
| **Question design bias** | Questions designed by framework author | Pre-register expected bundles; negative control; independent adopter questions later |
| **Single-project generalization** | One repo cannot validate general model | Feasibility only; two independent repos required for Evidence Review |
| **Runtime/tool variance** | Cursor results may not transfer | Claim scoped to Cursor unless replicated |
| **Handoff bootstrap confound** | Session 0 refresh improves continuity independent of arbitration | Log Session 0 separately; baseline uses same Handoff state |
| **Hawthorne / demand characteristics** | AI may comply because rules are explicit | Baseline without adapter on same questions |

**Can claim if successful:** Minimum sufficient context on `jon-ohio-portfolio`, in Cursor, maintainer-operated sessions.

**Cannot claim alone:** Cross-project, cross-tool, or independent-adopter generalization.

---

## Expected bundles by question type

| Question | Responsibility | Expected minimum bundle |
|----------|----------------|-------------------------|
| "What changed recently?" | Session continuity | `ai/handoff.md` only |
| "Why was dark theme made the default?" | Decision rationale | `docs/adrs/ADR-073-*.md` (Handoff only if needed to locate) |
| "Why was ADR-073 accepted?" | Decision rationale | ADR-073 only — negative control: Handoff not required first |
| "What's in scope for WIP badge work?" | Implementation scope | Handoff horizon → ADR-073 / relevant paths |

**Pass on precision:** bundle matches expected minimum (no missing, no unnecessary artifacts).

---

## Pass threshold

- ≥3 treatment sessions with context precision + sufficiency met
- Average bundle smaller than baseline
- Negative-control session passes (ADR without Handoff-first overfit)
- Stop condition not triggered

Handoff-before-git is logged but not primary pass criteria.

---

## Session log

| Session | Type | Question / action | Responsibility | Expected bundle | Actual bundle | Count | Precision | Sufficiency | Git? | Handoff before git? | Failure layer | Notes |
|---------|------|-------------------|----------------|-----------------|---------------|-------|-----------|-------------|------|---------------------|---------------|-------|
| 0 | Setup | Observation bootstrap | Session continuity | Handoff update | ai/handoff.md | 1 | Y | Y | N | N/A | none | Handoff refreshed 2026-07-01 |
| 1 | Treatment | Summarize uncommitted FigJam work | Implementation scope | Handoff + changed paths | ai/handoff.md, FigJamEmbedFrame.tsx, AnnotatedFigure.tsx | 3 | Y | Y | N | N/A | none | Horizon named files; no git log |
| 2 | Treatment | "What changed recently?" | Session continuity | Handoff only | ai/handoff.md | 1 | Y | Y | N | Y | none | Delta answers question completely |
| 3 | Negative control | "Why was ADR-073 accepted?" | Decision rationale | ADR-073 only | docs/adrs/ADR-073-case-study-progress-status-dark-default-homepage-headline.md | 1 | Y | Y | N | N | none | Handoff not loaded first — control passed |
| 4 | Treatment | "Why was dark theme the default?" | Decision rationale | ADR-073 | docs/adrs/ADR-073-*.md | 1 | Y | Y | N | N | none | Option D in ADR sufficient |
| 5 | Baseline | Repeat Session 2, ignore arbitration | Session continuity | Handoff only (ideal) | git log, git status, git diff, handoff.md, ADR-073, ADR-074, FigJamEmbedFrame.tsx, AnnotatedFigure.tsx | 8 | N | Y | Y | N | none | Unconstrained recall; over-fetched |

---

## Results vs predictions

_Filled 2026-07-01 after Sessions 0–5._

| Prediction | Expected | Actual | Met? |
|------------|----------|--------|------|
| Average context bundle size | Smaller than baseline | Treatment avg 1.5 files vs baseline 8 | Y |
| Context precision | Higher than baseline | 4/4 treatment precise; baseline imprecise | Y |
| Git access | Less frequent | Treatment: 0 git; baseline: git log/status/diff | Y |
| Task success | No decrease | All sessions answered correctly | Y |
| Human clarification | Lower | N/A — maintainer-operated single operator | — |
| Handoff trust (proxy) | Higher | Session 2 answered from Handoff alone | Y |

## Stop condition fired?

**No.** No consecutive sessions required bundle expansion beyond protocol recommendation.

## Responsibilities sub-test (optional)

_Not run._ Deferred to post-review if independent adopter replicates.

---

## Conclusion

**Maintainer experiment — preliminary positive signal.** Delegated responsibility resolution produced smaller, precise context bundles on `jon-ohio-portfolio` in Cursor (Sessions 1–4). Negative control (Session 3) loaded ADR-073 without Handoff-first overfit. Baseline (Session 5) exhibited unconstrained recall (8 artifacts vs 1).

**Does not generalize** without independent adopter replication per threats to validity.

**Pass threshold:** Met for maintainer feasibility test. Proceed to observational phase and independent adopter replication; do not freeze framework identity until Position Paper + adopter gate.

---

## Observational phase

**Phase:** Open after controlled Sessions 0–5 (2026-07-01).

Use **normal work on `jon-ohio-portfolio`** — no synthetic probes. Record field observations during real Cursor sessions. Overrides are evidence; do not tune protocol during Evidence Window.

| Date | Task (normal work) | Adapter feel | Bundle override? | Why override | Responsibility failure? | Observation ran? | Handoff updated? | Notes |
|------|-------------------|--------------|------------------|--------------|-------------------------|------------------|------------------|-------|
| 2026-07-02 | Phase open — no `jon-ohio-portfolio` sessions logged | N/A | N | | N | N | N | Observational phase active; record during normal portfolio work in Cursor |

**Record when:**

- Adapter felt invisible or intrusive
- Proposed bundle was overridden (and why)
- Responsibility misclassified repeatedly (note failure layer)
- Handoff stayed current via Observation — or didn't
- Context selection felt faster or slower than pre-adapter habit
- Question did not map cleanly to four responsibilities

**Instrument reuse:** This protocol + worksheet is portable. Independent adopters can run the same columns on their project; compare experiments, not anecdotes.
