# Pre-Event Freeze

## Problem

Event-driven engines can silently rewrite predictions or rationale after new information arrives. This destroys the audit value of prediction registers and makes post-mortems weak.

## When To Use

Use this pattern when an engine has a known decision event:

```text
FOMC statement / vote
ODAC meeting / vote
FDA decision date
NVDA earnings release
policy announcement
court ruling
```

## Minimal Artifacts

```private artifact```

## Workflow

```text
1. Select the candidate prediction.
2. Confirm resolution criteria and invalidation signals.
3. Attach all evidence available before freeze time.
4. Attach consensus baseline available before freeze time.
5. Record probability and rationale.
6. Mark the artifact as frozen.
7. After event, resolve against pre-declared criteria.
8. Write post-mortem without editing the frozen artifact.
```

## Human Gate

The freeze must be explicitly accepted by a human owner if the prediction will be used for calibration.

## Domain-Specific Extension Points

```text
FOMC: meeting id, statement diff baseline, dissent baseline, sell-side or market-implied consensus.
ODAC: case id, FDA/sponsor briefing document timestamp, vote question, panel roster.
AI_CAP: source placeholders, release/transcript availability, sell-side baseline, approval packet.
IDN_NI: policy event id, local/English source split, execution indicator snapshot.
```

## Failure Modes

```text
freeze_after_leak: Freeze occurs after material information has already entered.
moving_resolution_target: Resolution criteria are changed after the event.
consensus_absent: No baseline exists, so gap claims become ungrounded.
overfreezing: Engine freezes too many low-value predictions and creates paperwork drag.
```

