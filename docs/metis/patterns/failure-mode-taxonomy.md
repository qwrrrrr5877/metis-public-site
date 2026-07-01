# Metis Failure Mode Taxonomy

This taxonomy merges the to-self failure modes already identified in Metis with heuristic-system failure modes highlighted by "Learning Beyond Gradients".

Use it during:

```text
weekly review, for active issues
monthly compression review, for accumulated debt
annual meta-calibration, for structural risks
Core change review, for cross-engine risks
```

## 1. Narcissistic Loop

The engine produces polished versions of beliefs the owner already wanted to believe.

Defense:

```text
prediction resolution
competing hypotheses
adversarial input
explicit counter-evidence fields
```

## 2. Tool-Building As Procrastination

Framework maintenance crowds out actual prediction generation and resolution.

Defense:

```text
weekly packet counts
time-log, when needed
primary weekly outcome
active engine limit
```

## 3. Premature Lock-In

The owner becomes reluctant to change a framework because too much identity or effort is invested in it.

Defense:

```text
legacy boundary
framework debt left intentionally
adopted_with_local_variant decisions
```

## 4. Knowledge Dies With You

Future self cannot reload the reasoning chain from artifacts.

Defense:

```text
inheritability test
evidence-bound beliefs
reasoning memos
golden cases
```

## 5. Self-Deception Scaffolding

Rules appear strict but contain escape hatches that always allow preferred conclusions.

Defense:

```text
Ulysses constraints
human review decisions
explicit exception logs
pre-event freeze
```

## 6. Drift From Ground Truth

The engine becomes internally coherent but less predictive of real-world outcomes.

Defense:

```text
calibration review
resolved predictions
error attribution
golden case regression
```

## 7. New Rule Breaks Old Case

A new pattern, belief, parser, or gate improves a recent case while breaking an important past case.

Defense:

```private artifact```

## 8. Memory Poisoning

Low-quality or misread evidence becomes repeatedly cited and contaminates beliefs, lessons, or cross-engine patterns.

Defense:

```text
source reliability
evidence quality scoring
evidence decay or revalidation
primary-source preference
linked-evidence audit
```

## 9. Prediction Definition Gaming

Predictions are defined so softly that they become easy to mark as correct without learning.

Defense:

```text
closeable criteria
freeze boundary
third-party or Core review
wrong_reason_profit error attribution
```

## 10. Cross-Engine API Drift

One engine changes the meaning of a shared artifact, field, rule, or pattern while another engine still relies on the old meaning.

Defense:

```text
metis_manifest.yaml
Core change notes
metis_compatibility_log.csv
domain_outputs vs core_outputs separation
```

## 11. Big Ball Of Mud

The engine has many logs, beliefs, lessons, and rules, but the structure is too coupled to safely modify.

Defense:

```text
history compression review
coupling complexity audit
legacy boundary
pattern promotion discipline
```

## Review Prompt

During review, ask:

```text
Which of the 11 failure modes is currently most likely for this engine?
What artifact would reveal it early?
What is the smallest defensive action?
```

