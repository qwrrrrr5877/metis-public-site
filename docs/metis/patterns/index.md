# Metis Workflow Patterns

Patterns are reusable workflow shapes, not universal domain rules.

A pattern should describe:

```text
problem
when to use
minimal artifacts
workflow
human gate
domain-specific extension points
failure modes
```

Promotion rule:

```text
Do not promote a pattern to Core merely because it worked once in one engine. Promote it when at least one other engine can plausibly use the workflow shape while keeping its domain-specific checks local.
```

