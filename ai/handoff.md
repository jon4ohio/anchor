# Handoff

**Contract:** Handoff  
**Problem coordinated:** What changed recently? What's next?

**Updated:** 2026-06-29

---

## Delta

Phase 1 boundary clarifications shipped. Adoption validation active—framework research, not framework development. Published as `v0.1.1-validation`.

## Horizon

1. Adoption validation — first adopter; dual observation log per [Validate Through Use](playbooks/validate-through-use.md)
2. Greenfield validation — Start Project Playbook

## Next

- First adopter — finish real work without changing Anchor; log friction
- Post-project review question after each session

## Blocked

None.

## Questions *(empirical — defer to usage)*

- **Research:** Does boundary reduce re-orientation while adopters evolve independently?
- **Skill hypothesis:** transferable coordination expertise — current exemplar is what-to-keep
- **Boundary hypothesis:** durable context ends at framework contracts — ADR-003 deferred until observed evidence

## Roadmap

- **Milestone:** Foundation Complete
- **Active phase:** Adoption validation (first adopter)
- **Out of scope:** Framework changes without two-project evidence; ADR-003 before adoption evidence; CLI; editor adapters

---

## Friction Log

| Date | Repeated explanation | Contract | Root cause | Action |
|---|---|---|---|---|
| 2026-06-28 | `ai/` directory may confuse strangers (sounds AI-specific) | — | Hypothesis — defer until evidence | Observe: if two independent adopters ask "why is everything under ai/?", propose rename with evidence |
| 2026-06-29 | Should tooling/routing live in Anchor? | — | Boundary hypothesis — not decided | Watch during adoption: boundary vs contract-use observations |

**Graduation rule:** Unchanged items after three cycles promote or delete.

**Post-project review:** What repeated coordination problem wasn't handled cleanly by existing contracts?
