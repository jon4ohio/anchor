# Handoff

**Contract:** Handoff  
**Problem coordinated:** What changed recently? What's next?

**Updated:** 2026-07-02

---

## Delta

- **Audience-Specific Expressions architecture** — [POSITION-audience-specific-expressions](../docs/decisions/POSITION-audience-specific-expressions.md); practices as organizing mechanism, not eighth contract
- **docs/practices/** — catalog ([README](../docs/practices/README.md)), [project-orientation](../docs/practices/project-orientation.md), [contributing-evidence](../docs/practices/contributing-evidence.md) methodology
- **journey/README.md** — Reference Projects as proving ground; bridge to independent adoption → evidence → evolution
- **Cross-links** — CONTRIBUTING Practices section, evidence.md methodology link, glossary (Practice, audience-specific expression), Framework Reference, Ch. 6, observation template
- **Gap fixes** — Ch. 6 as learning expression (methodology page separate); Skill column in catalog; playbook ↔ practice links; governance methodology link; anchor-site in journey index; README Contribute link

## Horizon

1. **PR 2 — anchor-site** — demonstrate Ch. 6 lifecycle in [anchor-site](https://github.com/jon4ohio/anchor-site); first observations via Observation Guide
2. **anchor-lab recruitment** — 3–5 independent users; synthesis before Anchor citations
3. **Independent adopters** — orient-project Branch A + Branch B; record in [evidence.md](../releases/v0.2/evidence.md)
4. **Full Evidence Review** — when exit checklist clears → [decision.md](../releases/v0.2/decision.md)

## Next

- Distribute anchor-lab recruitment link per [recruitment.md](https://github.com/jon4ohio/anchor-lab/blob/main/docs/recruitment.md)
- Invite two independent orient-project adopters (Branch A + B)
- Record `jon-ohio-portfolio` observational sessions in [context-arbitration-experiment.md](../releases/v0.2/context-arbitration-experiment.md#observational-phase)

## Blocked

- **Full Evidence Review** — requires 2 independent adopter repositories + anchor-lab synthesis (see [decision.md](../releases/v0.2/decision.md))

## Roadmap

- **Release:** v0.2 shipped; Evidence Window **open**
- **Focus:** Recruitment → evidence collection → full Evidence Review → Decision
- **Out of scope:** Major redesign; eighth contract; Entry §4 rewrite

---

## Friction Log

Contract-level framework friction. Product observations during open window → [releases/v0.2/evidence.md](../releases/v0.2/evidence.md).

| Date | Repeated explanation | Contract | Root cause | Action |
|---|---|---|---|---|
| 2026-06-28 | `ai/` directory may confuse strangers | — | Hypothesis | Observe: two adopters ask → propose rename |
| 2026-06-29 | Should tooling/routing live in Anchor? | — | Boundary hypothesis | Watch during adoption |
| 2026-06-30 | README was framework-first | Experience | Product layer missing | **Resolved v0.2** |
| 2026-06-30 | start-project greenfield-only | Playbook | Paths conflated | **Resolved v0.2** — orient-project |
| 2026-06-30 | jon-ohio-portfolio (existing validation): 74+ ADRs may intimidate newcomers | Experience | Scale vs complexity | Observe if repeated twice |

**Graduation rule:** Unchanged items after three cycles promote or delete.

**Release Governance:** [current.md](../releases/current.md) · [governance.md](../releases/governance.md) · [v0.2 evidence](../releases/v0.2/evidence.md)
