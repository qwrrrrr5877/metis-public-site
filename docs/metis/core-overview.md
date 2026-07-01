# Metis Core

Metis Core is the private coordination layer for Metis-class engines.

It does not replace engine-specific ledgers. It defines the minimal shared interface that lets multiple engines report status, expose rules, and share progress without forcing domain-specific knowledge into a universal schema.

## Directory Layout

```text
schemas/      Shared minimal field contracts
rules/        Private cross-engine operating rules
registries/   Portfolio and family registries
scripts/      Local dashboard and validation helpers
dashboard/    Generated portfolio views
changes/      Core change notes for engine compatibility review
patterns/     Reusable workflow shapes extracted from engines
templates/    Weekly review and new-engine scaffolds
```

## Core Principle

Engines do not exchange free-form thoughts. They exchange auditable events:

```text
belief_updated
prediction_opened
prediction_resolved
lesson_promoted
schema_exception_requested
cross_engine_candidate
engine_health_changed
```

Each engine remains domain-specific, but each must expose:

```text
metis_manifest.yaml
weekly_packet_template.yaml
prediction register
belief or concern ledger
evidence ledger
error attribution log
lesson registry, when available
```

When Core changes, add a small note under `changes/` instead of asking engines to reread the full charter. Engines should record adoption, local variants, or exceptions in `metis_compatibility_log.csv`.

When creating a new engine, start from `templates/new_engine_scaffold/` and keep the first scope narrow.
