---
name: r-hello-skill
description: Use when verifying that a skills manager (such as Vercel's) can discover and install a skill from this repository. A minimal end-to-end smoke-test skill that confirms installation, loading, and invocation all work.
---

# Hello Skill

## Overview

A minimal, self-contained skill used to confirm that a skills manager can
discover, install, load, and invoke a skill from this repository. If you can
read this content after invoking the skill, the install pipeline works.

## When to Use

- Verifying a freshly configured skills manager can pull skills from this repo
- Confirming a newly published skill becomes installable and invocable
- Smoke-testing the install → load → invoke path after changing repo structure

When NOT to use: real tasks. This skill does no work beyond confirming itself.

## What to Do

When invoked, respond with a short confirmation that includes:

1. The skill name (`r-hello-skill`)
2. A note that installation and invocation succeeded
3. The repository it was installed from, if known

Example response:

> ✅ `r-hello-skill` loaded successfully. The skills manager installed and
> invoked this skill from the personal skills repository.

That's it — no files to edit, no commands to run. Successful invocation IS the
passing test.
