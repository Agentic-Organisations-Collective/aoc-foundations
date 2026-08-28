# aoc-foundations — Operating Instructions

## Tasks Are GitHub Issues

Resolution of the 2026-08-26 board meeting: **to-dos are created as an issue in this
repo** — not as a markdown list, not in an external to-do app. Whoever identifies a
task creates it directly, instead of writing it into a file.

Belongs here: the reusable building blocks themselves — brand kit, the canonical field
list of the membership application, templates, schemas, taxonomies, body profiles. How
a form is implemented → `aoc-website`. *That* the membership process runs this way is
management → `aoc-board`.

**This repo is public.** Whatever isn't meant for the public also doesn't belong in an
issue text here.

An issue names the occasion, the concrete task, and the preconditions. The owner
assigned is whoever took on the task — when unclear, better nobody than the wrong
person. Tasks from a meeting carry `sitzung:<YYYY-MM-DD>` and reference the minutes in
the footer.

Where the field list, web form, and issue template must be changed together, the
issues reference each other across repos instead of being duplicated.

This applies alongside the content conventions below: open points on a content file
still go into the `issues.md` next to it — it only becomes a *task* once it's a GitHub
issue.

## Content Conventions

- **Content markdown = content only.** Content files (boilerplate, messaging, copy)
  contain exclusively the texts — no intros, provenance, explanations, or open points.
  Open points/meta go into an `issues.md` next to the content file. READMEs may
  explain.
