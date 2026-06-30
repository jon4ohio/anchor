# SPEC-001: Export command

## Problem coordinated

Export tasks as JSON for backup or migration.

## Requirements

- `tasklight export` writes all tasks as JSON to stdout
- Output includes id, title, completed flag
- Must not mutate the database

## Acceptance

- [ ] Export on empty DB returns `[]`
- [ ] Export after add returns correct JSON array

## References

- [ADR-001](../decisions/ADR-001-sqlite.md) — storage format unchanged
