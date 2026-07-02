# Contributing Evidence

*How your experience helps Anchor evolve.*

---

You've built something.

You've worked with Anchor.

You now know something that nobody else did before you started.

This chapter is the handoff back to the framework—not feedback, but evidence.

---

## Two ways to contribute

Every adopter contributes in two ways:

- by building software with Anchor;
- by helping Anchor learn from that experience.

The second contribution is optional, but it is how the framework continues to improve.

---

## Closing the Loop

Anchor isn't complete when a project begins using it.

The lifecycle closes when observations from real projects help improve the framework for future adopters.

```text
Read → Understand → Adopt → Build → Observe → Contribute Evidence → Anchor Evolves
```

After adoption, you enter the **Delivery Loop**—normal engineering with Handoff, ADRs, and Specs. When something about Anchor itself stands out, you can enter the **Evidence Loop** and share what you observed. Reference projects and teaching artifacts feed the **Learning Loop**, improving adoption for everyone who follows.

---

## Three loops

Anchor coordinates three related cycles. They overlap, but each has a distinct responsibility.

### Delivery Loop

You're delivering software.

```text
Build → Observe → Improve Project
```

This is everyday work on your project. Update Handoff between sessions. Record ADRs when decisions constrain future work. Write Specs when scope is bounded. See [Adopt Anchor](04-building-your-own.md) and [Project Entry §4](../project/entry.md).

### Evidence Loop

You're improving Anchor.

```text
Observe → Contribute Evidence → Anchor Evolves
```

When you notice friction, missing guidance, or something that worked surprisingly well—share it. Maintainers look for **repeated patterns** across projects before changing the framework. This chapter describes how.

### Learning Loop

You're improving adoption.

```text
Reference Projects → Examples → Better Adoption
```

Teaching artifacts—like the [Canonical Journey](../../journey/john-ohio/README.md) and [Reference Projects](examples.md)—help future adopters learn faster. Your observations can improve those artifacts too.

---

## Why evidence matters

Anchor evolves through evidence gathered from real projects—not through opinions in isolation.

Ask what **happened**, not whether someone liked a feature:

- What became easier?
- What remained difficult?
- Where did context break down?
- What documentation was missing?
- Which parts of Anchor were most useful?
- Which parts were unnecessary?

This matches [Release Governance](../../releases/governance.md): record friction and confidence, not satisfaction surveys.

---

## What to observe

Use these prompts when something stands out during normal work. You do not need to answer all of them.

**Friction** (from [Release Governance](../../releases/governance.md)):

- What confused you?
- What felt unnecessary?
- What did you expect that didn't happen?
- What did you understand without explanation?

**Confidence**:

- What did you trust without needing to verify?
- When did you stop feeling like you had to reconstruct the project?
- Was there a moment you could simply continue?

For detailed observation methodology, see [Contributing Evidence practice](../practices/contributing-evidence.md). For a structured capture format, see the optional [Observation Guide](templates/observation-guide.md).

---

## Where evidence comes from

Evidence is collected in different **validation environments**—each answers a different question. See the [glossary](glossary.md#validation-environments) for definitions.

| Environment | Question it answers |
|---------------|---------------------|
| Reference Project | Does teaching match current best practice? |
| Existing Project | Does adoption work without migration? |
| Greenfield Project | Does day-one orientation work? |
| Independent Adoption | Does it generalize without maintainer control? |

**Evidence source**—who produced the observation—is a separate idea. A maintainer on a greenfield project and an independent adopter on an existing project produce different kinds of evidence. See [Evidence Source](glossary.md#evidence-source) in the glossary.

---

## Evidence levels

Not all observations carry the same weight. See [Evidence levels](glossary.md#evidence-levels) in the glossary.

Self-assessment is a **hypothesis** until independently corroborated. That is expected—share what you observed anyway.

---

## How to share

Keep the barrier low. Any of these work:

- **GitHub Discussions** on the [Anchor repository](https://github.com/jon4ohio/anchor)
- **Issues** describing what you observed—not a redesign proposal
- **Pull requests** that record evidence, when you have something concrete to add

If you'd like to capture observations while using Anchor, the [Observation Guide](templates/observation-guide.md) can help. It's entirely optional—the same observations can be shared through Discussions, Issues, or pull requests.

---

## Not every observation becomes a framework change

Every observation is valuable.

Some observations reveal documentation gaps.

Some suggest template improvements.

Some become future releases.

Some remain project-specific.

Anchor evolves by looking for repeated patterns across multiple projects rather than reacting to individual experiences.

---

## What happens next

When you share an observation, maintainers **record** it. They do not immediately change the framework.

```text
Observation → Discussion → Evidence → Decision → Release
```

During an open Evidence Window, observations go into the release `evidence.md`. At **Evidence Review**, maintainers ask what repeated, what confidence adopters gained, and whether change is justified.

Curious what happens next? See [Release Governance](../../releases/governance.md) to learn how observations become documentation improvements, ADRs, or future releases.

---

## See it in practice

Teaching artifacts show Anchor in different lights:

| Artifact | Teaches |
|----------|---------|
| [Canonical Journey](../../journey/john-ohio/README.md) | How one project evolved over time |
| [Reference Projects](examples.md) | Current best practice, live demonstration |
| Independent adoption | Generalization without maintainer involvement |

Browse [Examples](examples.md) for current instances.

---

## Thank you

Every project teaches something.

Some observations confirm that Anchor is working as intended. Others reveal gaps, rough edges, or opportunities to improve.

By sharing what you observed—not just what you think—you're helping Anchor evolve through the same evidence-driven approach it encourages for software projects.

Thank you for contributing to that journey.

---

[Experience index](README.md) · [Release Governance](../../releases/governance.md) · [Observation methodology](../practices/contributing-evidence.md) · [Practice catalog](../practices/README.md)
