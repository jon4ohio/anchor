# v0.2 Validation

Record observations from applying [orient-project](../../ai/playbooks/orient-project.md). Do not answer from theory.

---

## Validation questions

- Do "responsibility," "contract," and "continue instead of reconstruct" resonate?
- Where do adopters stall — Experience Ch 3 or Journey Session 2?
- Does the CLAUDE.md multi-responsibility example match real projects?

---

## Environments

| # | Repository | Branch | Status | Record |
|---|------------|--------|--------|--------|
| 1 | Anchor meta-repo | Existing | Complete | [Handoff](../../ai/handoff.md) 2026-06-30 |
| 2 | jon-ohio-portfolio | Existing | Orient assessment complete | [Portfolio worksheet](#portfolio-existing-project) |
| 3 | External #1 | Greenfield (Branch A) | Pending maintainer | — |
| 4 | External #2 | Existing (Branch B) | Pending maintainer | — |

---

## Portfolio (existing project)

**Repository:** `jon-ohio-portfolio`  
**Method:** orient-project Branch B — assess and classify only (no migration).

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
| `README.md` | Visitor + dev onboarding | Product page (visitors) / pointer to Entry | Keep split — matches v0.2 README pattern |
| `AGENTS.md` | Tool operating rules | Adopting-project (not Anchor contract) | Keep outside framework |
| Case study pages in `app/work/` | Intended behavior / narrative | Spec-like (per case study) | Project-specific — not Anchor framework |

### Orient — gaps

- Portfolio **already uses Anchor contracts** from prior adoption. orient-project Branch B confirms mapping — no eighth contract needed.
- `AGENTS.md` is not a Skill (tool dispatch) — boundary matches Anchor CONTRIBUTING exclusions.
- Journey Session 2 CLAUDE.md example applies to repos with bloated AI context; portfolio uses thin `AGENTS.md` + Entry — **variant path**, not contradiction.

### Continue — observation

Portfolio validates **overlay adoption**: mature ADR tree + Entry + Handoff without restructuring. Responsibility language maps cleanly.

**Friction:** ADR count (74+) may intimidate newcomers reading Experience before Entry — observe if adopters conflate "many ADRs" with "Anchor complexity" (log if repeated twice).

---

## Per-environment worksheet (template)

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

## Close criteria

- [x] Anchor meta-repo self-review
- [x] Portfolio orient assessment documented
- [ ] External greenfield repo (Branch A)
- [ ] External existing repo (Branch B) — beyond portfolio if second distinct project needed
- [ ] Friction log updated after external sessions
- [ ] v0.3 plan drafted from repeated observations only

**Note:** External repos #3–4 require maintainer-run sessions on distinct codebases. Worksheets and orient-project playbook are ready.
