# Week 06 — Testing and GitHub Actions

## Topic

Test plan, test cases, and GitHub Actions for Project 0.

---

## Testing Goal

The goal was to verify that the Two Sum function works correctly with different kinds of input.

The function receives an integer array and a target value, then returns two indices where the two numbers add up to the target.

---

## Test Case Categories

I prepared 20 main test cases divided into six categories:

1. Basic / normal cases
2. Negative numbers
3. Zero and boundary cases
4. Duplicate values
5. Large numbers
6. No-solution cases

---

## Example Test Cases

```text
[2, 7, 11, 15], target = 9
[-1, -2, -3, -4, -5], target = -8
[0, 0], target = 0
[3, 3], target = 6
[1000000000, -1000000000], target = 0
[1, 2, 3], target = 10
```

---

## Test Validation

The test file uses a helper function called `checkResult`.

It checks:

- The returned indices are valid.
- The two indices are different.
- The two values really add up to the target.
- The test result is printed clearly.

---

## GitHub Actions

I also connected the tests with GitHub Actions.

Workflow:

```text
Push code
↓
Compile C++ code
↓
Run tests
↓
Pass or fail result
```

The final workflow passed successfully.

---

## Reflection

This week helped me understand that testing is not only checking one example. A good test plan should cover normal cases, edge cases, and failure cases. GitHub Actions also showed how automated testing can make software development more reliable.