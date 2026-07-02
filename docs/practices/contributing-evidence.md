# Practice: Contributing Evidence

Record what happened when you use Anchor on a real project — friction and confidence — without redesigning the framework mid-flight.

---

## Audience-specific expressions

| Expression | Artifact | When to use |
|---|---|---|
| Learning | [Contributing Evidence (Ch. 6)](../experience/06-contributing-evidence.md) | Why evidence matters, three loops, how to share |
| Methodology | This page | How to observe well — friction, confidence, source tagging |
| Execution | [validate-through-use playbook](../../ai/playbooks/validate-through-use.md) | Research friction through natural project work |
| Evidence | [v0.2 evidence log](../../releases/v0.2/evidence.md) | Where to record observations during open window |
| Reference | [anchor-lab](https://github.com/jon4ohio/anchor-lab) | Independent validation experiments |

---

## When to use

- You adopted Anchor on a real project (new or existing)
- An Evidence Window is open ([current release](../../releases/current.md))
- You want to contribute observations that may inform framework evolution

You do not need to be validating Anchor as your primary goal. Work normally. Notice what happens.

---

## What counts as evidence

| Type | Description | Example |
|---|---|---|
| **Friction** | Something confused, blocked, or required re-explanation | "I expected Handoff to be read first; AI ignored it" |
| **Confidence** | Something worked without reconstruction | "I trusted Entry and continued without re-explaining the project" |
| **Hypothesis** | Plausible pattern, not yet confirmed twice | "Ch. 4 delegation section may reduce adoption friction" |

**Observations** are specific and behavioral. **Opinions** ("Anchor should have X") belong in issues only after recording what actually happened.

Record first. Maintainers decide actions at Evidence Review — not during the window.

---

## How to observe

### 1. Do normal work

Work on the project as you would without Anchor. Do not force framework usage to "validate" it.

### 2. Pause when explaining

When you catch yourself re-explaining something, pause and ask:

> Which contract owns this?

If nothing owns it yet, note it. If it repeats, log it.

### 3. Create contracts only when natural

Write Specs or ADRs when real decisions or scope boundaries appear — not preemptively.

### 4. Log observations

Add rows to the current release [evidence.md](../../releases/v0.2/evidence.md) observations log.

Use structured source tags in the `Source` column only (not in prose):

| Tag | Environment |
|---|---|
| `meta` | Anchor meta-repo |
| `validation-existing` | Existing mature repository |
| `greenfield` | New project from day one |
| `independent` | External adopter outside maintainer control |

See [Glossary — Validation environments](../experience/glossary.md#validation-environments).

### 5. Update Handoff after sessions

If you are working in a project using Anchor contracts, update [Handoff](../../ai/handoff.md) delta for session continuity. Evidence and Handoff serve different purposes — do not conflate them.

---

## Friction questions

Go beyond the checklist. Be specific:

- What confused you? What did you expect instead?
- What felt unnecessary? Which step or document?
- What did you understand without explanation?
- Which contract were you looking for? Did you find it?
- Did you re-explain the same thing twice? What was it?

**Good:** "Branch B step 2b: I had 12 markdown files and wasn't sure which were coordination vs implementation."

**Weak:** "Documentation could be better."

---

## Confidence questions

- What did you trust without needing to verify?
- When did you stop feeling like you had to reconstruct the project?
- Was there a moment you could simply continue?
- Did Entry, Handoff, or an ADR answer a question before you asked it?

---

## What not to do

- Do not redesign Anchor while observing — record observations; propose changes at Evidence Review
- Do not force framework usage to generate evidence
- Do not treat a single session as proof — repetition across projects matters for framework changes
- Do not open structural PRs during an open Evidence Window ([CONTRIBUTING.md](../../CONTRIBUTING.md))

**Maintainer response during open window:**

> We're in an Evidence Window. Please record the observation in [evidence.md](../../releases/v0.2/evidence.md). Changes will be considered at Evidence Review.

---

## Pairing with other expressions

| Expression | Role |
|---|---|
| [Ch. 6](../experience/06-contributing-evidence.md) | Learning — why evidence matters, three loops, how to share |
| This page | Methodology — how to observe well |
| [validate-through-use playbook](../../ai/playbooks/validate-through-use.md) | Execution — prescribed step order for research validation |

Use Ch. 6 for the newcomer journey. Use this page for observation methodology. Use the playbook when you need sequential execution steps.

---

## Governance

- [Release Governance](../../releases/governance.md)
- [Evidence Window exit conditions](../../releases/governance.md#evidence-window)
- [CONTRIBUTING.md](../../CONTRIBUTING.md)

---

## Related

- [Practices catalog](README.md)
- [POSITION-audience-specific-expressions](../decisions/POSITION-audience-specific-expressions.md)
