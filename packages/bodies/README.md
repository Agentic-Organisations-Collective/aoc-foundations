# bodies

Canonical roster of the association's governing bodies — one small Markdown
profile per person (name, role, LinkedIn, short bio DE + EN, image reference).
The people counterpart to `messaging` (verbal identity) and `brand-kit` (visual
identity): who represents the collective, kept in one place instead of being
re-typed on the website, in press material, or on event programs.

## Contents

- `board/` — the three board members (Vorstand: chair, deputy chair, treasurer)
- `curatorium/` — curatorium members (Kuratorium; advisory body, § 10 Satzung)
- `portraits/` — portrait images, one per person, filename = profile slug
- `issues.md` — open points (unconfirmed details)

## Consumers

- **Website** (`aoc-website`) — the "Über uns" `PeopleGrid` blocks (Vorstand +
  Kuratorium); published into the site's live content.
- **Press / event programs** (`aoc-communications`) — speaker/organiser bylines
  where the same person appears.

## Governance

Shared read across repos. The formal election record (who holds which office,
Wahlergebnis, Satzungsbezug) lives in `aoc-board` (register); this package
holds the public-facing bio text derived from it, not the register itself.
