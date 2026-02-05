# Self-Critique Prompting Pattern

## Purpose

Self-critique prompting asks the model
to evaluate and improve its own output.

It introduces a second internal review phase.

---

## When should you use it?

Use this pattern when:

- output quality is critical
- hallucinations are costly
- design or architectural decisions are generated

---

## Structure

A typical self-critique prompt consists of two phases:

1. generate the initial answer
2. critically review the answer and propose improvements

---

## Software architecture example

Task:
Propose an authentication architecture for a web application using JWT.

Instruction:
First, propose a solution.
Then, review your solution and list weaknesses, risks, and missing parts.

---

## Strengths

- improves completeness
- reveals hidden assumptions
- often catches obvious mistakes

---

## Limitations

- does not guarantee correctness
- still depends on model knowledge
- increases response length
