# Candidate Registration Gate

## Problem

Engines receive many hunches, candidate evidence items, and plausible prediction targets. Without a gate, weak signals enter formal ledgers too early and pollute calibration.

## When To Use

Use this pattern when a signal needs to graduate into one of:

```text
registered prediction
promoted belief
formal evidence row
active lesson
thesis candidate
```

## Minimal Artifacts

```text
candidate id
candidate type
linked evidence
consensus or baseline status
required checks
lesson or precedent recall
human decision
decision notes
```

## Workflow

```text
1. Capture the candidate without making it binding.
2. Identify required evidence and missing baseline.
3. Recall relevant lessons, precedents, or prior misses.
4. Run domain-specific checks.
5. Produce a registration recommendation.
6. Human owner decides: register, defer, reject, or request more evidence.
7. If registered, create the formal ledger row.
8. If rejected or deferred, preserve decision notes for future calibration.
```

## Human Gate

The final transition from candidate to registered artifact requires human ownership. LLM output can propose but not register final judgment by itself.

## Domain-Specific Extension Points

```text
FOMC: active lesson recall, voter linkage, meeting baseline, candidate registration gate.
AI_CAP: candidate evidence promote/reject, source archive validation, consensus baseline review.
ODAC: clinical-stat gate, precedent validity conditions, briefing tone checks.
IDN_NI: actor/institution linkage, four-indicator execution check, source reliability check.
```

## Failure Modes

```text
rubber_stamp_gate: Gate exists but approves everything.
overstrict_gate: Useful rare targets are blocked because no prior lesson exists.
lesson_absence_confused_with_invalidity: No recalled lesson should mean "needs review", not automatic rejection.
domain_logic_leakage: Core gate tries to encode domain-specific expertise and becomes brittle.
```

