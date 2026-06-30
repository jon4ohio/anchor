# Adopt Anchor

Anchor doesn't replace your documentation. It helps you coordinate what you already have.

Keep your ADRs, architecture docs, and AI context files. Clarify what each piece owns. Add only the coordination pieces you're missing.

---

## What you'll have at the end

After your first adoption session, you'll have:

- A clear project identity — where contributors orient in under five minutes
- Clear ownership of key knowledge — decisions, scope, and session continuity each have an owner
- A way to continue between sessions — without reconstructing context from chat history

Plan for one focused session. Most projects map what they already have in a single sitting.

---

## What you'll do

1. **Understand your project as it exists today** — list what already coordinates the project (docs, ADRs, AI context, conventions).
2. **Decide what each piece of knowledge is responsible for** — identity, decisions, scope, session state, or something else.
3. **Add only the coordination pieces you're missing** — create contracts where no owner exists; trim overlap in AI context files.
4. **Continue working normally** — update Handoff between sessions.

---

## Choose your path

### I have an existing project {#existing-project}

You have docs, ADRs, AI context files, or team conventions. Map what exists before introducing anything new. Fill gaps only.

**Next step:** [Orient Project — Branch B](../../ai/playbooks/orient-project.md#branch-b-existing-project)

### I'm starting a new project {#new-project}

You have little to discover. Establish project identity and first bounded scope. Skip decision records until a real decision constrains work.

**Next step:** [Orient Project — Branch A](../../ai/playbooks/orient-project.md#branch-a-new-project)

---

## Already have ADRs or `CLAUDE.md`?

Keep them. Anchor maps ownership—it does not migrate files. See [Responsibilities](03-responsibilities.md) for how mixed AI context files separate into owners.

---

## Want more?

- **See a real example:** [See Anchor in practice](../../journey/john-ohio/README.md)
- **Framework vocabulary** (Assess → Classify → Orient → Continue): [Framework Reference](05-framework-reference.md)
