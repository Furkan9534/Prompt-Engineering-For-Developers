# Foundations – Core Principles of Prompt Design

This section introduces the foundational design approach
used throughout the entire repository.

The goal is not to obtain a good answer once,
but to design prompts that can be controlled and reproduced.

---

## Why do we need a foundation?

In real systems, prompts are:

- often ambiguous
- written by different people
- modified over time
- executed through APIs

As a result, several problems emerge:

- the model role is unclear
- task boundaries are not well defined
- available information is not specified
- output formats become unstable

Therefore, prompt design cannot be treated as free-form writing.

---

## Core design principles

The following principles are used throughout this repository.

### 1. Clarity

What the model is expected to do
must be stated in a way that leaves no room for ambiguity.

---

### 2. Explicit boundaries

It must be clear:

- what the model is allowed to use
- what assumptions it can make
- what scope it should stay within

---

### 3. Structural design

A prompt should be treated as a structured artifact,
not as a plain block of text.

---

### 4. Output control

The generated output should be:

- suitable for downstream systems
- stable in format
- ideally machine-parsable

---

## A prompt is an interface

A prompt acts as an interface between
your application and the language model.

A poorly designed interface leads to:

- misuse
- unpredictable behavior
- higher maintenance costs

For this reason, prompts should be treated
as contracts.

---

## The smallest meaningful structure

In this repository, the smallest meaningful prompt structure
consists of four components:

- Role
- Task
- Context
- Output

This structure forms the foundation of
all prompt patterns introduced later.

Detailed explanations of these components
are provided in the
`role-task-context-output` directory.

---

## Prompt design is an iterative process

A good prompt is not discovered in a single attempt.

The following loop should be applied continuously:

1. design
2. run
3. evaluate
4. improve

This loop will be formalized later
in the evaluation and iteration section.

---

## What will you be able to do after this section?

After completing this section, you will be able to:

- decompose prompts into explicit components
- clearly separate role, task, context and output
- design prompts that are maintainable and extensible
