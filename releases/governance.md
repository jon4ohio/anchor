# Release Governance

Permanent definition of how Anchor evolves after a release ships.

---

## Canonical rule

> **During an Evidence Window, contributors record observations. Maintainers decide actions only after Evidence Review.**

Contributions are welcome — in the form of observations, not redesigns.

**How to observe:** [Contributing Evidence methodology](../docs/practices/contributing-evidence.md)

---

## Lifecycle

```text
Release
    ↓
Evidence Window open
    ↓
Evidence Review
    ↓
Decision
    ↓
Next State
```

**Next State** (one of):

- **Continue current release** — no new release required
- **Patch release** — editorial or small fixes
- **Minor release** — incremental product change
- **Major redesign** — structural change; planning warranted

No assumption that Major redesign happens. Evidence leads somewhere; it does not assume semver.

---

## Evidence Window

### While open

- Contributors **record** observations in the release `evidence.md` — see [observation methodology](../docs/practices/contributing-evidence.md)
- Maintainers **do not** implement structural changes from single reports
- Issues and PRs proposing structural change: record observation; defer action to Evidence Review

### Maintainer response template

> We're in an Evidence Window. Please record the observation in [evidence.md](v0.2/evidence.md). Changes will be considered at Evidence Review.

(Current instance path updates per release.)

### Exit conditions (all required)

1. Adoption evidence from **at least two independent repositories** (minimum one non-author adopter), via [orient-project](../ai/playbooks/orient-project.md).
2. Observations recorded in release `evidence.md` — friction **and** confidence.
3. **Evidence Review** completed (three questions below).
4. `decision.md` filed with **Next State** and reason.

Then close the window in `release.md`.

---

## Evidence Review

Ask only:

1. What **repeated** observations did we collect?
2. What **confidence** did users gain?
3. Does the evidence justify changing the product?

### Observations vs actions

Evidence Review produces two outputs in `decision.md` — never conflated during the window:

| Observation | Action |
|-------------|--------|
| Three adopters opened Journey before README | Move Journey CTA higher |
| Nobody misunderstood "responsibility" | No change |

Record observations first. Decide actions only at review.

---

## Friction questions (unbiased)

Ask adopters:

- What confused you?
- What felt unnecessary?
- What did you expect that didn't happen?
- What did you understand without explanation?

Do not ask: "Did you like responsibility?" — that biases the outcome.

---

## Confidence questions (promise validation)

- What did you trust without needing to verify?
- When did you stop feeling like you had to reconstruct the project?
- Was there a moment you could simply continue?

---

## Freeze during Evidence Window

| Frozen | Allowed |
|--------|---------|
| Structural product changes (Journey map, Experience chapters, playbook steps) | Editorial copy (README headlines if meaning unchanged) |
| Framework contracts (Entry §2–§5, seven contracts) | Typos, broken links |
| Core promises and frozen vocabulary for that release | |

**Rule:** Semantic and structural changes wait for Evidence Review. Editorial maintenance may proceed during the window.

Per-release `release.md` records only **Evidence Window: open | closed** and dates — not this table.

---

## Shared pattern

Framework, Product, and Release all follow:

```text
Observe → Record → Look for repetition → Promote only when earned
```

---

## Templates

[releases/templates/](templates/) — instantiate per release.

---

## Using Anchor?

If you're adopting Anchor in your own project, see [Experience → Contributing Evidence](../docs/experience/06-contributing-evidence.md) for guidance on sharing observations. This document describes how maintainers evaluate evidence; the Experience guide explains how adopters contribute it.
