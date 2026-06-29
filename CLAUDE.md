# Personal Skills Repository

This repo is a standalone collection of personal agent skills, managed and
installed via Vercel's skills manager.

## Layout

- Each skill lives in `skills/<base-name>/SKILL.md` (plus optional supporting
  files). The directory uses the bare base name (no prefix) — e.g.
  `skills/hello-skill/`.
- `SKILL.md` frontmatter requires `name` and `description` per the
  [agentskills.io spec](https://agentskills.io/specification).

## Naming Convention

- **Prefix every skill's frontmatter `name` with `ran:`** (e.g.
  `ran:hello-skill`). The prefix applies to the `name` field only — the skill
  directory uses the bare base name (`skills/hello-skill/`), since authorship is
  already implied by this repo.
- Rationale: standalone skills install into a flat namespace keyed by `name`,
  with no per-author scoping. The `ran:` prefix namespaces skills authored in
  this repo (mirroring the `plugin:skill` convention) and avoids collisions with
  third-party skills of the same base name.

## Goals

- **Migrate skill management here.** The long-term goal is to stop tracking and
  installing skills via the dotfiles repo (`~/Dev/dotfiles/.agents/skills/`) and
  instead manage all personal skills from this repo, installed through Vercel's
  skills manager.
- Until migration is complete, the dotfiles `.agents/skills/` may still hold the
  active installed skills. Treat this repo as the source of truth going forward.

## Local Development

- TBD — decide on a case-by-case basis. (Note: installs are one-time copies,
  decoupled from this repo, so editing a skill here does not update an already
  installed copy; reinstall or symlink for live iteration.)
