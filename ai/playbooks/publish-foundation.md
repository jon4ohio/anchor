# Playbook: Publish Foundation

**Contract:** Playbook  
**Problem coordinated:** How do we publish the Foundation milestone to GitHub?

---

## Promise

Prescribe execution order for publishing Anchor Foundation to a remote repository.

---

## Prerequisites

- Foundation refinement complete and committed locally
- [contract-ownership Review](../reviews/contract-ownership.md) passing
- GitHub repository created or URL confirmed

---

## Steps

### 1. Confirm local state

Working tree clean. Foundation refinement commit on `main`.

### 2. Create GitHub repository

Create a new repository on GitHub (or confirm existing URL).

### 3. Add origin remote

```bash
git remote add origin <github-url>
```

Skip if `origin` already configured.

### 4. Push main

```bash
git push -u origin main
```

### 5. Tag Foundation release

```bash
git tag -d v0.1-bootstrap 2>/dev/null
git tag v0.1.0-foundation
git push origin v0.1.0-foundation
```

### 6. Create GitHub release

- **Title:** Anchor Foundation
- **Tag:** `v0.1.0-foundation`

Release notes:

- Seven contracts, four principles, collaboration lifecycle
- Self-hosting framework with passing ownership audit
- Minimal Experience scaffolding + glossary
- Framework frozen until cross-project evidence

```bash
gh release create v0.1.0-foundation --title "Anchor Foundation" --notes "..."
```

### 7. Verify repository

- README renders correctly
- Tags visible on GitHub
- Release exists with correct title and tag

Update [Handoff](../handoff.md) delta after publish completes.

---

## References

- [Project Entry](../../docs/project/entry.md)
- [ADR-002: Framework vs Experience](../../docs/decisions/ADR-002-framework-vs-experience.md)
- [Validate Through Use](validate-through-use.md)
