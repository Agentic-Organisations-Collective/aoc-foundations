# Contributing to `aoc-foundations`

How anyone works in this repository — human or AI agent. There is no second
rulebook: `CLAUDE.md`, `AGENTS.md`, `GEMINI.md`, and
`.github/copilot-instructions.md` all point here. Everything an agent needs to
know belongs in this file.

## Language: This Repository Is English

Everything written into this repository is **English** — documentation, READMEs,
handbooks, processes, specs, decision records, schemas, field lists, file and folder
names, issue and pull request text, and commit messages.

This is independent of the language you speak with your AI agent. Several of us work in
German with our agents, and that is fine — but German must not land in the repo. If you
drafted in German, translate before it lands.

Four exceptions, and only these:

- **Verbatim evidence.** Quotes, transcripts, and copies of emails or letters keep their
  original wording. What surrounds them — framing, summary, commentary — is English.
- **Minutes** of German-language meetings, including the narrative and long-form
  versions. They record what was said. The issues derived from them are English.
- **Legally binding texts** in `aoc-governance`. The German version is the binding one;
  an English translation sits alongside it without binding force.
- **Outward-facing content for a German-speaking audience** — member communication,
  website copy, announcements. The published text is German; everything *about* it
  (briefs, review notes, READMEs, issues) is English.

In doubt: English. An exception covers the artifact itself, never the work around it.
Existing German files are backlog, not precedent — they are migrated deliberately, never
as a side effect of an unrelated change.

Decided 2026-09-01, replacing the earlier rule that minutes, issues, and commit messages
were German.
The building blocks here are consumed across repos and by third parties: English
throughout, including field names, keys, and schema identifiers. A German label shipped
into a form is content, not documentation — the label may be German, the field name
around it is not.

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

## Commits and Pull Requests

- **Commit messages are English**, a short line describing the change. No ticket prefix —
  there is no Jira here. Reference an issue via `(#12)` at the end of the line.
- **AI co-authorship is disclosed.** Agentically produced commits carry the trailer with
  the concrete model name, not a generic "Claude":

  ```
  Co-Authored-By: Claude Opus 5 <noreply@anthropic.com>
  ```

  The association is testing agentic work; that a commit came about this way is part of
  the subject matter and is not hidden. Purely manual commits do not carry the trailer.
  Decided 2026-08-26.
- **Do not push and do not create a branch unasked.** Commit with a targeted pathspec,
  never `git add -A`.

---

## One File, Several Names

This file is the whole rulebook for working in this repository. `CLAUDE.md`,
`AGENTS.md`, `GEMINI.md`, and `.github/copilot-instructions.md` are symlinks pointing
here — whichever agent you run, it reads this file. **Never create a second rulebook
under one of those names**; add what you have to say here instead.

Org-wide rules that apply across all AOC repos: [`.github/CONTRIBUTING.md`](https://github.com/Agentic-Organisations-Collective/.github/blob/main/CONTRIBUTING.md)
