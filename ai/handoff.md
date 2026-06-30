# Handoff

**Contract:** Handoff  
**Problem coordinated:** What changed recently? What's next?

**Updated:** 2026-06-30

---

## Delta

Release Governance shipped: `releases/` layer with governance.md, templates, v0.2 instance.

## Horizon

1. **Evidence collection** — independent adopters (see [evidence.md](../releases/v0.2/evidence.md))
2. **Evidence Review** → Decision → Next State ([decision.md](../releases/v0.2/decision.md))

## Next

- Independent greenfield + existing repo orient sessions
- Record observations in releases/v0.2/evidence.md (not structural PRs during open window)

## Blocked

None.

## Roadmap

- **Release:** v0.2 shipped; Evidence Window **open**
- **Focus:** Evidence collection → Evidence Review → Decision
- **Out of scope:** Major redesign planning; eighth contract; Entry §4 rewrite

---

## Friction Log

Contract-level framework friction. Product observations during open window → [releases/v0.2/evidence.md](../releases/v0.2/evidence.md).

| Date | Repeated explanation | Contract | Root cause | Action |
|---|---|---|---|---|
| 2026-06-28 | `ai/` directory may confuse strangers | — | Hypothesis | Observe: two adopters ask → propose rename |
| 2026-06-29 | Should tooling/routing live in Anchor? | — | Boundary hypothesis | Watch during adoption |
| 2026-06-30 | README was framework-first | Experience | Product layer missing | **Resolved v0.2** |
| 2026-06-30 | start-project greenfield-only | Playbook | Paths conflated | **Resolved v0.2** — orient-project |
| 2026-06-30 | Portfolio: 74+ ADRs may intimidate newcomers | Experience | Scale vs complexity | Observe if repeated twice |

**Graduation rule:** Unchanged items after three cycles promote or delete.

**Release Governance:** [current.md](../releases/current.md) · [governance.md](../releases/governance.md) · [v0.2 evidence](../releases/v0.2/evidence.md)
