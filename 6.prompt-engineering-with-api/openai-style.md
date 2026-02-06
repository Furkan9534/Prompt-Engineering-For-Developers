# Prompt Engineering in API-based Systems

This document describes a typical API-oriented
prompt engineering workflow.

---

## Separation of system and user instructions

A recommended structure:

- system message:
  defines global behavior and rules
- user message:
  contains task-specific input

---

## Template-based prompting

Prompts should be defined as templates
with explicit variables.

This allows:

- reuse
- testing
- and version control.

---

## Prompt lifecycle

A production prompt typically goes through:

- design
- offline evaluation
- limited rollout
- monitoring
- refinement

---

## Observability

In API-based systems,
prompt behavior should be observable through:

- logs
- quality metrics
- failure cases
