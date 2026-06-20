# Personal Skills Repository

This repo is a standalone collection of personal agent skills, managed and
installed via Vercel's skills manager.

## Layout

- Each skill lives in `skills/<name>/SKILL.md` (plus optional supporting files).
- `SKILL.md` frontmatter requires `name` and `description` per the
  [agentskills.io spec](https://agentskills.io/specification).

## Naming Convention

- **Prefix every skill name in this repo with `r-`** (e.g. `r-hello-skill`).
  This applies to both the directory name and the frontmatter `name` field.
- Rationale: standalone skills install into a flat namespace keyed by `name`
  (`~/.agents/skills/<name>/`), with no per-author scoping. The `r-` prefix
  marks skills authored in this repo and avoids collisions with third-party
  skills of the same base name.

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
