# Architectural Position Paper: Context Arbitration

## Status

**Proposed** — pending Evidence Review and independent adopter validation.

**Not an ADR.** Do not treat as accepted framework identity until gated review completes.

**Governance path:** Evidence Window → Evidence Review → this paper → one more adopter → ADR (if evidence supports).

---

## Evidence reviewed

- **Date:** 2026-07-01 (maintainer experiment only — independent adopters pending)
- **Validation project (existing) experiment:** [context-arbitration-experiment.md](../../releases/v0.2/context-arbitration-experiment.md) — conducted on `jon-ohio-portfolio`
- **Independent adopters:** Pending

---

## Summary

Maintainer falsification experiment (Sessions 0–5) on `jon-ohio-portfolio` in Cursor:

- Treatment sessions: context precision and sufficiency met; average bundle 1.5 files
- Baseline (unconstrained): 8 artifacts; imprecise for continuity question
- Negative control: ADR-073 loaded without Handoff-first overfit
- Stop condition: not fired
- Predictions: 5/5 applicable predictions met

**Claim scope:** Feasibility on one repo, one runtime, maintainer-operated. Not generalization.

**Supported now:** Capability — delegated responsibility resolution may produce minimum sufficient context (maintainer feasibility, one repo, Cursor).

**Not supported yet:** Identity — Anchor as responsibility-coordination framework.

**Next:** Observational phase on `jon-ohio-portfolio` (normal work) → independent adopter (highest-value evidence) → Evidence Review → one adopter validates without reading this paper → ADR if evidence supports.

---

## Position (draft — held until evidence)

> **Anchor coordinates responsibility.**
>
> Responsibilities determine protocols.  
> Protocols determine persistence.  
> Contracts preserve durable outcomes.

**Product differentiator (candidate):** Context arbitration — given many possible truths, determining which truths are relevant for the current moment of work.

**User outcome:** Continue instead of reconstruct.

---

## Three protocols

| Protocol | Purpose | Output |
|----------|---------|--------|
| Orientation | Resolve who owns the current question | Responsibility |
| Session | Given responsibility, assemble bounded context | Context bundle |
| Observation | Determine whether responsibility moved | Persistence actions |

---

## Adapter pattern

```
Framework  → defines protocol (responsibility rules + steps)
Adapter    → invokes protocol at lifecycle boundaries
Tool       → implements invocation (Cursor, Claude Code, CI, human checklist)
```

Adapters are adopting-project concerns per CONTRIBUTING. Framework does not ship editor rules.

---

## Failure attribution

| Layer | Failure |
|-------|---------|
| Responsibility | Wrong owner selected |
| Protocol | Correct owner, wrong context rules |
| Adapter | Correct protocol, poor execution |

---

## Explicit non-claims

- Responsibilities as named Entry §2 layer — TBD by sub-test
- Eighth contract — not proposed
- Cross-tool generalization without replication
- Generalization from single maintainer experiment

---

## What would falsify this position

- Context precision not improved vs baseline
- Negative control shows Handoff habit, not responsibility resolution
- Stop condition triggered twice consecutively
- Independent adopter cannot reproduce bounded context without author-designed questions

---

## Next steps

1. ~~Complete validation project (existing) controlled experiment on `jon-ohio-portfolio`~~ — done 2026-07-01
2. **Observational phase** — record field observations during normal work ([worksheet](../../releases/v0.2/context-arbitration-experiment.md#observational-phase))
3. **Independent adopter** — highest-value evidence; minimal explanation; own project; own questions
4. Evidence Review per [governance.md](../../releases/governance.md)
5. If supported: draft ADR superseding implicit v0.1 product framing (minor release)

---

## Related

- [releases/v0.2/context-arbitration-experiment.md](../../releases/v0.2/context-arbitration-experiment.md)
- [releases/v0.2/evidence.md](../../releases/v0.2/evidence.md)
- [ADR-001](ADR-001-contracts-not-artifacts.md)
