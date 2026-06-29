# Agentic Organisations Collective — Brand Identity Guidelines

_Official brand documentation for the non-profit association (Verein)._

This guide is the single source of truth for the Agentic Organisations Collective visual identity.
All assets referenced here live alongside this document in the
[`brand-kit`](../README.md) package.

## Table of contents

1. [Brand essence & positioning](#1-brand-essence--positioning)
2. [The logo mark: the "Collective Node"](#2-the-logo-mark-the-collective-node)
3. [Color palette: "Fresh Innovation"](#3-color-palette-fresh-innovation)
4. [Typography stack](#4-typography-stack)
5. [Visual applications & layout logic](#5-visual-applications--layout-logic)
6. [Asset reference](#6-asset-reference)

---

## 1. Brand essence & positioning

The **Agentic Organisations Collective** is an agile, practitioner-driven non-profit association
(Verein) designed to bridge the gap between AI hype and enterprise reality. It
functions as a collaborative "concept-hardening forge" where tech leaders
stress-test next-generation automation and Software Factory architectures.

### Core principles to maintain

- **Strictly contribution (no spectators):** The brand must feel like an active
  workshop, not a passive, corporate broadcast.
- **The protected space (Geschützter Raum):** Visuals should reinforce security,
  mutual trust, and high-level peer-to-peer consulting.
- **Human-centric engineering:** Balancing hardcore enterprise automation
  architectures with the authentic, human connection of an independent collective.

---

## 2. The logo mark: the "Collective Node"

The logo abstracts complex network topologies into a streamlined, highly
recognizable emblem.

![Agentic Organisations Collective logo](../logo/agentic-organisations-collective-logo.svg)

- **Geometry:** Three primary nodes arranged in a stable triangle, symbolizing
  the foundational threshold of a resilient community network.
- **The central "O":** Thick, organic, curved lines connect the three points and
  intersect in the center to form an abstract letter **"O"** (for Organisations).
- **Usage rule:** The mark is highly versatile and must always be usable in full
  monochrome (solid white on a dark background, or solid dark blue/black on a
  cream canvas).

---

## 3. Color palette: "Fresh Innovation"

This palette avoids standard corporate rigidity, blending high-energy tech
signals with warm, approachable community tones.

| Element | Color name | Hex | Purpose / application |
| :-- | :-- | :-- | :-- |
| **Primary accent** | Electric Cobalt Blue | `#1D4ED8` | Dominant brand mark color, links, primary buttons, and focal points. |
| **Supporting accent** | Aurora Green | `#34D399` | Secondary highlights, status indicators, and innovation callouts. |
| **Primary canvas** | Papyrus Cream | `#F8F4E6` | Default background for web interfaces, documents, and event spaces. |
| **Text & contrast** | Slate Black | `#334155` | Body text, subtle borders, and structural interface elements. |

---

## 4. Typography stack

To ensure global accessibility across open-source web assets and community
portals, the type system relies on a **single open-source typeface**
([Google Fonts](https://fonts.google.com/)) — one coherent voice, self-hosted.

### One-font system: Outfit

The brand uses **Outfit for everything** — display and text alike. Hierarchy and
contrast come from **weight and scale**, not a second family. (A two-font pairing
with a similar grotesk such as Inter or Hanken Grotesk was tested and rejected: the
contrast against Outfit was too low to justify a second face.)

- **Tone:** Modern, geometric, and dynamic — clean, low-contrast letterforms with
  even, friendly proportions. It signals to incoming CTOs and architects a
  forward-looking, engineering-driven collective without corporate stiffness.
- **Weight ladder:**
  - **Bold 700** — the logo wordmark ("AGENTIC ORGANISATIONS COLLECTIVE"), H1/H2
    headings, and high-impact calls to action.
  - **Medium 500** — subheadings, navigation, and UI labels.
  - **Regular 400** — paragraph / running text and the core claim/tagline
    (_"driving next-gen automation, agentic architectures, and enterprise
    governance"_).
- **Self-hosting:** ship the woff2 files with the asset (latin subset) rather than
  loading from a third-party CDN — keeps public pages GDPR-clean and offline-robust.

---

## 5. Visual applications & layout logic

**The contrast rule:** When designing the public content area or the secure
closed-members portal, always lead with structural clarity. Let **Outfit Regular /
Medium** do 90% of the heavy lifting for readability, using **Outfit Bold** (display
headings, the wordmark) and **Electric Cobalt Blue** as deliberate, high-impact
accents to draw the eye to core community actions (e.g., "Join the Association" or
"Submit an Abstract").

---

## 6. Asset reference

| Asset | Path |
| :-- | :-- |
| Primary logo (vector) | [`logo/agentic-organisations-collective-logo.svg`](../logo/agentic-organisations-collective-logo.svg) |
| Logo on blue background | [`logo/agentic-organisations-collective-logo-blue.png`](../logo/agentic-organisations-collective-logo-blue.png) |
| Logo on transparent background | [`logo/agentic-organisations-collective-logo-transparent.png`](../logo/agentic-organisations-collective-logo-transparent.png) |
| Mood board | [`mood-board/agentic-organisations-collective-mood-board.png`](../mood-board/agentic-organisations-collective-mood-board.png) |
