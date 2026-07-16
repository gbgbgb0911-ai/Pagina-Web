# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Current state

This repository is effectively empty. As of this writing it contains only:

- `README.md` — currently a single blank line (no content yet).
- `CLAUDE.md` — this file.

There is **no source code, build system, dependency manifest, test suite, linter, or CI configuration yet**. Do not assume any framework, package manager, or toolchain is present — none has been chosen. Verify the tree (`git ls-files`) before acting on any assumption about the stack.

The repository name is `Pagina-Web` ("página web" is Spanish for "web page"), which indicates the intended purpose is a website. The concrete stack (static HTML/CSS/JS, a framework such as React/Vue/Astro, a static-site generator, etc.) has not been decided.

## Working in this repository

Because the project is being started from scratch, the first substantive change will define its conventions. When you scaffold or add the initial stack:

- Prefer the tooling the user requests. If unspecified, ask before committing to a framework or package manager, since that decision shapes everything downstream.
- **Update this file** as soon as real structure exists — replace the sections below with the actual build/lint/test commands and an architecture overview, so future instances aren't working blind.

Once a toolchain is in place, this file should document at minimum:

- **Build** — how to produce a production build.
- **Run / dev server** — how to start the app locally.
- **Test** — how to run the full suite and a single test.
- **Lint / format** — the commands and any enforced style.
- **Architecture** — the big-picture structure that requires reading multiple files to grasp.

## Git conventions

- Default branch: `main`.
- Development for the current task happens on branch `claude/claude-md-docs-co5f3h`; push there, not to `main`.
