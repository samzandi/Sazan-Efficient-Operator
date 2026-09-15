# Sazan Efficient Operator

A reusable execution-policy skill for AI agents: less token waste, less repetition, fewer unnecessary interruptions, and evidence-based completion without sacrificing quality.

## What it optimizes

- Minimal unnecessary output and context repetition
- Direct execution when intent and permissions are clear
- Questions only for genuine blockers
- Consecutive safe steps without approval loops
- Targeted retrieval instead of broad context reloads
- Incremental edits instead of regenerating unchanged work
- Evidence before completion or production-ready claims
- Security and quality controls preserved at all times

## Install / Use

Use `SKILL.md` as the canonical skill definition. Other project or domain skills can reference it as their execution-policy layer:

```text
Execution policy: apply sazan-efficient-operator for token-efficient execution, minimal interruption, evidence-based completion, and concise reporting.
```

## Modes

`balanced-efficient` is the default. `ultra-compact` is useful for repetitive execution. `diagnostic` allows more detail when troubleshooting requires it.

## Design principle

Token efficiency is not answer reduction. The objective is to remove waste while retaining everything necessary for a correct, safe, verified deliverable.
