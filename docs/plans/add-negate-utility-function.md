# Plan: Add Negate Utility Function

## Goal

Create a `negate` utility function in `src/negate.ts` that exports `negate(n: number): number`, which returns `-n`.

## Tasks

### Task 1: Implement the negate utility function

**Agent:** coder
**Depends on:** none

Create `src/negate.ts` with the following implementation:

```typescript
export function negate(n: number): number {
  return -n;
}
```

**Acceptance criteria:**
- `src/negate.ts` exists and exports a function named `negate`
- `negate(n: number): number` takes a number and returns its negation (`-n`)
- `negate(5)` returns `-5`, `negate(-3)` returns `3`, `negate(0)` returns `0`
- Changes must be on a feature branch with a GitHub PR created via `gh pr create`

### Task 2: Add tests for the negate utility function

**Agent:** coder
**Depends on:** Task 1

Add unit tests to verify the `negate` function behaves correctly.

**Acceptance criteria:**
- A test file (e.g., `src/negate.test.ts`) exists with tests for the `negate` function
- Tests cover: positive input, negative input, and zero
- All tests pass
- Changes must be on a feature branch with a GitHub PR created via `gh pr create`

## Task Dependencies

```
Task 1 (implement negate) → Task 2 (add tests)
```

Task 2 depends on Task 1 because tests must import the function being tested.
