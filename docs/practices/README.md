# Practices

> **Organizational documentation — not a framework contract.**

For maintainers and contributors organizing repeatable engineering activities in Anchor.

Newcomers do not need this page. Start with [Experience](../experience/README.md): Learn → Adopt → Build → Contribute.

---

## What this is

A **practice** is a reusable engineering activity — project orientation, contributing evidence, contract ownership.

Each practice may have **audience-specific expressions**: the same knowledge expressed differently for learning, execution, verification, or demonstration.

See [POSITION-audience-specific-expressions](../decisions/POSITION-audience-specific-expressions.md) for the architectural proposal.

**Philosophy:**

> A practice is the reusable engineering activity. Documentation, playbooks, skills, reviews, and reference projects are different expressions of that same practice for different audiences and purposes.

---

## Practice catalog

| Practice | Page | Learning | Execution | Verification | Skill | Reference |
|---|---|---|---|---|---|---|
| **Project Orientation** | [project-orientation](project-orientation.md) | [Ch. 4 Adopt Anchor](../experience/04-building-your-own.md) | [orient-project](../../ai/playbooks/orient-project.md) | [contract-ownership](../../ai/reviews/contract-ownership.md) | — | [john-ohio](../../journey/john-ohio/README.md) |
| **Contributing Evidence** | [contributing-evidence](contributing-evidence.md) | [Ch. 6](../experience/06-contributing-evidence.md) · [methodology](contributing-evidence.md) | [validate-through-use](../../ai/playbooks/validate-through-use.md) | — | — | [v0.2 evidence](../../releases/v0.2/evidence.md), [anchor-lab](https://github.com/jon4ohio/anchor-lab) |
| **Contract Ownership** | — | [Ch. 3](../experience/03-responsibilities.md), [Ch. 5](../experience/05-framework-reference.md) | — | [contract-ownership](../../ai/reviews/contract-ownership.md) | [what-to-keep](../../ai/skills/what-to-keep.md) | [john-ohio sessions](../../journey/john-ohio/README.md) |
| **Publish Milestone** | — | — | [publish-foundation](../../ai/playbooks/publish-foundation.md) | — | — | Anchor meta-repo [releases](../../releases/) |
| **Context Arbitration** *(experimental)* | — | — | — | — | — | [experiment log](../../releases/v0.2/context-arbitration-experiment.md) |

Empty cells mean no expression exists yet — not a gap to fill preemptively.

---

## Expression types

| Expression | Audience |
|---|---|
| Experience chapter | People learning Anchor |
| Playbook | Contributors executing a workflow |
| Review | Reviewers verifying quality |
| Skill | Specialized judgment-heavy execution |
| Reference project | Everyone through demonstration |

Playbooks live under `ai/` for historical reasons. They are practice expressions, not AI-only artifacts.

---

## Reference Projects

Reference Projects are the proving ground — where practices are demonstrated, validated, and evidenced.

See [journey/README.md](../../journey/README.md).

---

## Contributing

- **Record observations:** [contributing-evidence](contributing-evidence.md)
- **Propose framework changes:** [CONTRIBUTING.md](../../CONTRIBUTING.md)
