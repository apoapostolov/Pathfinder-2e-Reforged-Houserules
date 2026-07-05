# AGENTS.md - Pathfinder 2e Reforged Houserules

**Project-specific operating contract.** This repository holds the canonical
drafts for Pathfinder 2e houserules, player-facing references, and supporting
notes.

## Project Identity

- **Purpose**: Maintain a clear, versioned ruleset for Pathfinder 2e Reforged
  houserules.
- **Canonical source**: Treat `README.md` and any future rules files as the
  authoritative source for current rules text.
- **Scope**: Mechanical changes, explanations, examples, and changelog-style
  notes that support the houserules document set.

## Working Rules

- Keep rules text direct, readable, and mechanically precise.
- Prefer one rule per bullet when documenting behavior.
- Preserve old versions by archiving instead of deleting when material may be
  useful later.
- Use absolute dates (`YYYY-MM-DD`) in any operational notes or logs.
- Keep public content free of secrets, private campaign data, and unpublished
  personal information.

## Source Hierarchy

1. Explicit user instruction in the current session.
2. This `AGENTS.md`.
3. The repository `README.md` and any rules files.
4. Surrounding documentation and established repo patterns.
5. External rules references only when local context is insufficient.

## Change Protocol

- Edit files in place rather than creating duplicate variants.
- Regenerate any derived Markdown or reference files if they are added later.
- Run `markdownlint-cli2 --fix` on changed Markdown files before finishing.

## Last reviewed

`2026-07-05`.
