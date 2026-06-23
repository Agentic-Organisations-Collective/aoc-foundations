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
