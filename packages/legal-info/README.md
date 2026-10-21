# legal-info

Canonical register/legal identity data of the association — the structured
counterpart to `messaging` (verbal identity) and `brand-kit` (visual identity):
legal name, legal form, seat, register court and number, representation rule, and
the current board as entered in the register.

Source of truth for the facts is the official register extract filed in
`aoc-board/packages/register/founding/correspondence/`; this package holds the
same facts in a structured, reusable form so every consumer references one copy
instead of retyping it.

## Contents

- `register.md` — the canonical facts (name, legal form, seat, register court and
  number, representation, board, charitable-status flag).

## Consumers

- **Website** (`aoc-website`) — Impressum (§ 5 TMG): legal name, address, register
  court and number, represented by.
- **Press / official correspondence** (`aoc-communications`) — legal-entity line in
  letterheads and boilerplate where required.

## Governance

Shared read across repos; this repo is public. `register.md` deliberately omits
board members' place of residence and date of birth — part of the official
register entry, but not needed by any consumer here and not repeated in a public
repo beyond what's required; those particulars stay on file in the official
register extract in `aoc-board` (board-only). Updates follow a change in the
actual register entry, not the other way round.
