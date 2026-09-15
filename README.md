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

`SKILL.md` is the canonical runtime definition. Keep it small and load it as the execution-policy layer rather than copying the full policy into every project.

Other project or domain skills can reference it with one line:

```text
Execution policy: apply sazan-efficient-operator for token-efficient execution, minimal interruption, evidence-based completion, and concise reporting.
```

### OpenAI Skills API

OpenAI supports project-level reusable Skills with versioned skill content. Package this repository's skill files as a directory or ZIP and create the skill through the Skills API. Subsequent changes should be published as new skill versions and promoted by updating the default version.

This repository remains the source of truth; the OpenAI-hosted Skill is the installed runtime copy.

## Modes

`balanced-efficient` is the default. `ultra-compact` is useful for repetitive execution. `diagnostic` allows more detail when troubleshooting requires it.

## Design principle

Token efficiency is not answer reduction. The objective is to remove waste while retaining everything necessary for a correct, safe, verified deliverable.
