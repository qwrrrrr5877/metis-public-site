# History Compression Review

## Source Inspiration

This pattern was inspired by Jiayi Weng's "Learning Beyond Gradients" and its distinction between absorbing feedback and compressing history in heuristic systems.

Metis engines already absorb feedback through evidence, prediction resolution, error attribution, lessons, weekly packets, and dashboards. This pattern prevents those artifacts from growing into an unmaintainable pile.

## Problem

An engine that only records more evidence, predictions, lessons, and exceptions will eventually become hard to maintain. It may remember many things, but in a form that is too coupled, redundant, or local to guide future judgment.

## When To Use

Use this pattern monthly or quarterly for active engines, and after major event cycles for event-driven engines.

Examples:

```text
FOMC after two meeting cycles
AI_CAP after an earnings cycle
ODAC after three replay cases
IDN_NI after an RKAB resolution window
```

## Minimal Artifacts

```private artifact```

## Workflow

```text
1. Collect new feedback since the last compression review.
2. Identify repeated errors, repeated lessons, stale hunches, and redundant beliefs.
3. Check whether local patches should be:
   - deleted
   - merged
   - downgraded
   - promoted to a family/Core pattern
   - preserved as domain-specific local logic
4. Run golden cases mentally or mechanically against proposed simplifications.
5. Record which history was compressed and which debt remains.
6. Update weekly packet or monthly review with the compression decision.
```

## Human Gate

Compression changes judgment memory. A human owner must approve deletion, merging, promotion, or downgrade of material beliefs, lessons, gates, or schema variants.

## Domain-Specific Extension Points

```text
FOMC: merge overlapping statement-wording and minutes lessons only after checking meeting-cycle examples.
AI_CAP: separate durable thesis lessons from event runbook mechanics.
ODAC: preserve disease/endpoint boundaries when merging lessons.
IDN_NI: preserve local actor/institution path distinctions when compressing RKAB cases.
```

## Failure Modes

```text
overcompression: A useful local distinction is erased too early.
undercompression: Every patch is preserved and the engine becomes too coupled.
false_universalization: A domain-specific lesson is promoted to Core.
golden_case_neglect: Simplification breaks a known important case.
cosmetic_cleanup: Files are reorganized without reducing judgment complexity.
```

## Outputs

```private artifact```

