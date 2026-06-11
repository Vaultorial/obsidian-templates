---
type: resource
created: 2026-02-21
tags: [resource, web]
---

# Static Site Generators Overview

Reference note created while researching [[Personal Website Launch]]. Kept in Resources rather than the project folder because it will outlive the project — the next site rebuild will want it too.

## What a static site generator is

A tool that takes plain text files (usually Markdown) plus templates and produces a folder of finished HTML. No database, no server-side code at runtime — the output can be hosted anywhere that serves files.

## What I compared, and how it felt

- **Hugo** — single binary, very fast builds, templating takes getting used to.
- **Eleventy** — JavaScript-based, flexible, minimal assumptions about structure.
- **Astro** — component model, more moving parts than a five-page site needs.
- **Jekyll** — the veteran; fine, but I have no Ruby anywhere else in my life.

## Decision (2026-02-21)

Eleventy. Reason: my notes are already Markdown, I can read its templates without a manual, and the build is simple enough that future-me will still understand it in two years. Decision logged here so the project note ([[Personal Website Launch]]) stays about actions, not research.
