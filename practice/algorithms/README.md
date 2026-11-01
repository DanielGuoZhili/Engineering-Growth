# Dual-language Algorithm Practice (JavaScript + Python)

A lightweight, evidence-based learning track within [Engineering Growth](../../README.md).

## Purpose

Solve the **same algorithm problem independently in JavaScript and Python**, then compare the implementations and learn the transferable algorithm pattern. This complements—not replaces—the existing weekly engineering plan.

## Schedule and guardrails

- Minimum: **one practice session per week**; aim for **2–3 hours maximum**.
- Initially target **one problem per session**. An honest partial attempt counts.
- Keep the original English prompt; summarize **Input / Output / Constraints** in short English sentences before coding.
- Attempt both implementations yourself. Do not have an AI agent write a first attempt.
- Save both initial attempts *before* asking for a code review. Mark SOLO / HINTED / ASSISTED transparently.
- Prefer one pattern at a time (arrays & hashing, two pointers, stack, binary search, sliding window).
- Do not fill weeks of TODOs in advance. Adjust after the weekly review.
- Never commit employer/client source, sensitive data, or credentials.

## Learning resources

- Primary curated sequence: [Grind 75](https://www.techinterviewhandbook.org/grind75/).
- Run and submit JS/Python solutions: [LeetCode](https://leetcode.com/problemset/).
- Supplemental explanations *after your own attempt*: [NeetCode Roadmap](https://neetcode.io/roadmap).

## One-session workflow (120–180 minutes)

| Stage | Suggested duration | Evidence |
| --- | ---: | --- |
| English-first reading | 10 min | Input, Output, Constraints in your own words |
| JavaScript first attempt | 30–35 min | `solution.js` with honest status |
| Python first attempt | 35–40 min | `solution.py` with honest status |
| Test and reason | 20–30 min | Edge cases, complexity, optional alternative |
| Review and record | 20–25 min | `review.md` based on template |
| Flexible buffer | 0–40 min | Revisit or stop when time budget ends |

You may start with Python instead of JavaScript in a later week to avoid always relying on JS first; **each language's code must be written by you**, not pasted from an AI solution.

## Practice status

1. Choose the next item from [PROGRESS.md](PROGRESS.md).
2. Open the linked original English problem. Do **not** read the solution first.
3. Implement `solution.js` and `solution.py`; save your first attempt even when incomplete.
4. Run tests on LeetCode and note pass/fail and actual elapsed minutes.
5. Create `review.md` from [the template](_templates/review-template.md).
6. Share the two files and observations for an AI-assisted review **after** writing your attempt.
7. Update PROGRESS and link evidence in the relevant weekly review.

## Local workflow

Clone this repository on your own computer (see [the main README](../../README.md)), and edit the same files in VS Code, Cursor, or another editor. To sync:

```bash
git pull --ff-only
git status
git add practice/algorithms/
git commit -m "practice: dual-language algorithm attempt"
git push origin main
```

Do not run `git commit` when there are no changes. For conflicts or unexpected local changes, inspect `git status` rather than using `git reset --hard`.
