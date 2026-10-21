# Week 0 — Independent JS/TS Baseline 01

**Timebox:** 45 minutes. **Language:** JavaScript or TypeScript, your choice.

## Rules
- No Codex, ChatGPT, Copilot, internet searching for solutions, or generated code while attempting the task.
- You may use an editor, runtime, built-in debugger and language documentation (syntax only).
- Submit your own attempt even if unfinished; being honest is more valuable than passing all examples.
- After finishing, record actual minutes used, what you knew, what you struggled with, and whether you received help. You can request an AI review **after** saving your first attempt.

## Challenge: Most frequent valid event

You receive an array of event records. Each record has a `userId` and `action`. Return the `userId` that performed the most **valid** actions.

A record is valid only when:
1. `userId` is a non-empty string after trimming whitespace.
2. `action` is exactly `"click"` or `"view"` (case-sensitive).
3. An identical combination of trimmed `userId` and `action` is counted **once** per input array (deduplicate).

If several users have the same highest valid-action count, return the lexicographically smallest userId (JavaScript string comparison is acceptable). If there is no valid record, return `null`.

Implement:
```ts
type EventRecord = { userId: unknown; action: unknown };

function mostActiveUser(events: EventRecord[]): string | null {
  // Your code
}
```

If using JavaScript, omit the type annotations.

### Example
Input:
```json
[
  {"userId":" alice ","action":"click"},
  {"userId":"alice","action":"click"},
  {"userId":"alice","action":"view"},
  {"userId":"bob","action":"view"},
  {"userId":"bob","action":"click"},
  {"userId":"bob","action":"purchase"},
  {"userId":"","action":"click"}
]
```
Output: `"alice"` (both users have 2 distinct valid actions, so `alice` wins the tie).

### Test yourself
- Empty input returns `null`.
- Whitespace-only userIds, non-string userIds, uppercase `"Click"`, and unknown actions are ignored.
- Two identical valid records count once.
- Two different users with equal counts follow the tie-break rule.
- Input is not modified.

### What to submit
1. Your original implementation, e.g. `assessments/week0/mostActiveUser.ts` or `.js`.
2. At least 4 test cases written by you (inline assertions are fine).
3. In `assessments/baseline.md`, record time, assistance category (SOLO/ASSISTED/AGENT-BUILT), test results, one improvement you would make, and an explanation of time and space complexity.

### Assessment rubric (used in weekly review)
- Requirements and edge cases: 40%
- Correctness and tests: 35%
- Clarity and explanation: 25%

**Do not ask an agent to solve it before completing your first attempt.** Partial but authentic code is a valid submission.
