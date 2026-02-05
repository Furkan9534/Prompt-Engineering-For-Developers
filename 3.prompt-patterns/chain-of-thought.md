# Chain-of-Thought Prompting Pattern

## Purpose

Chain-of-thought prompting is used to guide the model
to solve problems through explicit intermediate reasoning steps.

The goal is to improve reasoning quality
by structuring the problem-solving process.

---

## When should you use it?

Use this pattern when:

- the task involves multi-step reasoning
- decisions depend on multiple constraints
- analysis or planning is required

---

## Structure

A typical chain-of-thought prompt requests:

- explicit assumptions
- intermediate reasoning steps
- and a final conclusion

---

## AI / data analysis example

You are designing a small data pipeline.

Task:
Decide whether a batch or streaming architecture is more suitable.

Constraints:
- data arrives every 5 minutes
- dashboards update every 30 minutes
- system complexity should be minimal

Instruction:
List assumptions, reason step by step, and conclude with your decision.

---

## Strengths

- improves logical coherence
- reduces missing intermediate steps
- helps debugging model behavior

---

## Limitations

- longer responses
- may expose unnecessary reasoning
- not ideal for simple tasks
