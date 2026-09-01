# aoc-foundations

Reusable neutral building blocks, kept separate from the domain-specific
operating repos. It provides shared building blocks that other repos can consume
without importing their own permission model.

## Packages

- `brand-kit` — visual identity assets and usage primitives
- `forms/member-application` — reusable membership application form template
- `templates` — shared neutral document templates
- `schemas` — validation schemas for structured artifacts
- `taxonomies` — shared vocabularies and classification models

## Governance

Shared read across repos. This repo should only contain things that can be
shared without crossing a permission boundary.

## Language

**Everything in this repository is written in English** — documentation, file names,
issues, pull requests and commit messages. That holds regardless of the language you
speak with your AI agent; working in German is fine, committing German is not.

Exceptions and full rule:
[CONTRIBUTING.md](./CONTRIBUTING.md#language-this-repository-is-english).

## Tasks

**To-dos are GitHub issues in this repository** — not markdown checklists, not an
external to-do app. Board resolution of 2026-08-26.

Belongs here: the reusable building blocks themselves — brand kit, the canonical field
list for the membership application, shared templates, schemas, taxonomies, the body
profiles. How a form is actually implemented goes to `aoc-website`; *that* the member
process works a certain way is management and goes to `aoc-board`.

**This repository is public.** Nothing that is not meant for the public belongs in an
issue here.

An issue names the occasion, the concrete task and its preconditions. Assign whoever
took the task on; where that is unclear, prefer no assignee over the wrong one. Tasks
from a meeting carry a `sitzung:<YYYY-MM-DD>` label and cite the minutes in a footer.

Where the field list, the web form and the issue template have to change together, the
issues reference each other across repositories rather than being duplicated.
