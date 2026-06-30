# ADR-001: SQLite for task storage

## Status

Accepted

## Context

John needed local persistence without running a server.

## Decision

Use SQLite via a single file at `~/.tasklight/tasks.db`.

## Consequences

- Simple backup (copy one file)
- No concurrent multi-user access (acceptable for personal CLI)
