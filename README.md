# Metis Public Site

This repository contains the public, sanitized website for Metis: a
multi-engine forecasting and thesis-building framework.

Metis is organized around independent domain engines that maintain their own
private working state, while sharing a small common core for manifests, progress
packets, reusable patterns, and portfolio-level review.

## What Is Published Here

This site is a public-facing layer, not the private system of record. It is meant
to share the framework and selected progress notes without exposing raw research
state.

Published materials may include:

- Metis core design notes
- public pattern-library pages
- sanitized portfolio dashboards
- selected weekly or build reports
- high-level engine descriptions

Private materials are intentionally excluded:

- raw belief ledgers
- raw prediction registers
- evidence and source archives
- closed schema details
- unresolved sensitive prediction internals
- private compatibility logs and human review notes
- trading, sizing, or position material

## Repository Structure

```text
.
├── docs/                  # MkDocs source pages
│   ├── index.md           # public home page
│   ├── dashboard/         # sanitized portfolio summaries
│   ├── metis/             # core framework and pattern library
│   └── reports/           # selected public reports
├── mkdocs.yml             # site navigation and MkDocs configuration
└── .github/workflows/     # GitHub Pages deployment workflow
```

## Site Generation

The contents of this repository are exported from a private Metis workspace by a
default-deny publication pipeline. Files are published only when they are
explicitly allowlisted or generated from approved summary fields. The public
export also redacts internal object identifiers, private artifact names, and
probability values from generated dashboard text.

Because this repository is generated, direct edits to `docs/` should be treated
as temporary unless they are also reflected in the private publication templates.

## Deployment

The site is built with MkDocs Material and deployed through GitHub Pages using
GitHub Actions.

On each push to `main`, the workflow:

1. installs MkDocs Material,
2. builds the static site,
3. uploads the generated `site/` artifact,
4. deploys it to GitHub Pages.

The repository should use `Settings -> Pages -> Build and deployment -> Source:
GitHub Actions`.

## Design Principle

The public site should explain the Metis method without becoming the Metis
memory. The private workspace remains responsible for calibration, evidence,
engine state, and decision history; this repository publishes only the parts
that are safe and useful to share.
