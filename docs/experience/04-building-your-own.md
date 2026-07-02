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

## Delegating adoption {#delegating-adoption}

You remain responsible for which changes to keep. An AI agent or human collaborator can execute the adoption procedure on your behalf.

Ask them to:

- follow the [Orient Project](../../ai/playbooks/orient-project.md) playbook;
- explain which adoption path they selected and why;
- preserve existing documentation, introducing only the coordination that's missing;
- show proposed changes before applying them.

Once adoption is complete, use [Working with AI](#working-with-ai) for normal project sessions.

---

## Already have ADRs or `CLAUDE.md`?

Keep them. Anchor maps ownership—it does not migrate files. See [Responsibilities](03-responsibilities.md) for how mixed AI context files separate into owners.

---

## Working with AI {#working-with-ai}

**AI follows the same orientation model as every other contributor.** See [Project Entry §4](../project/entry.md) (Understand phase).

If your project uses AI coding tools, provide a discoverable starting point that directs them to the project's canonical contracts. Keep this entry point as a dispatch layer rather than another source of project knowledge. Today, many projects implement this with files such as `AGENTS.md` or `CLAUDE.md`, but Anchor does not require a specific filename.

If your AI can read the repository, ask it to orient itself before starting work—Entry first; Handoff if continuing; relevant Spec or ADR for the task.

If repository access isn't available, provide only the minimum context needed—typically the Project Entry and current Handoff—rather than reproducing project documentation in the conversation.

Over time, you should rely more on the repository and less on pasted conversation context. If every session requires re-explaining Anchor, durable owners (Entry, Handoff, trimmed AI context files) need strengthening—not a longer chat prompt.

See [Responsibilities](03-responsibilities.md) for trimming overloaded `CLAUDE.md` or `AGENTS.md`.

---

## Want more?

- **See a real example:** [See Anchor in practice](../../journey/john-ohio/README.md)
- **Framework vocabulary** (Assess → Classify → Orient → Continue): [Framework Reference](05-framework-reference.md)
