# Release Governance

> **Not a framework contract.** Governs how Anchor itself evolves.

> **Looking for the current state of Anchor?** → [current.md](current.md)

Anchor has three governance layers:

| Layer | Governs | Instantiates |
|-------|---------|--------------|
| **Framework** | How projects coordinate knowledge | Entry, ADRs, contracts per repo |
| **Product** | How people discover and adopt | README, Journey, Experience |
| **Release** | How Anchor evolves | `releases/vX.Y/` per release |

**Symmetry:** Entry defines the framework; projects instantiate it. ADRs define decisions; individual ADRs instantiate them. **Release Governance defines the process; each release instantiates it.**

---

## Permanent documentation

- [governance.md](governance.md) — Evidence Window lifecycle, freeze rules, Evidence Review
- [templates/](templates/) — copy to start a new release instance

---

## Starting a new release

1. Copy `templates/` → `releases/vX.Y/`
2. Fill `release.md` when implementation ships
3. Open Evidence Window; record in `evidence.md`
4. Close window via Evidence Review → `decision.md`

See [governance.md](governance.md) for the full lifecycle.
