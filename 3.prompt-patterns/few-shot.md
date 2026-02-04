# Few-Shot Prompting Pattern

## Purpose

Few-shot prompting is used to demonstrate
the expected behavior and output format
by providing a small number of examples.

Instead of describing the rules,
the model learns the pattern from examples.

---

## When should you use it?

Use this pattern when:

- the output format is strict
- classification or transformation is required
- natural language instructions are insufficient to define the behavior

---

## Structure

A typical few-shot prompt consists of:

- multiple input–output examples
- followed by the new input to be solved

---

## Software engineering example

You are categorizing bug reports.

Example 1  
Input: API returns 401 after token refresh  
Output: Authentication / Authorization

Example 2  
Input: Page freezes when loading large dataset  
Output: Performance

Example 3  
Input: Null reference exception in user service  
Output: Backend logic

Now classify the following report:

Input: Dashboard crashes after filtering by date

---

## Strengths

- strong format consistency
- better control over labeling and classification
- reduces ambiguity

---

## Limitations

- examples must be carefully selected
- too many examples increase token usage
- hidden bias from examples may affect results
