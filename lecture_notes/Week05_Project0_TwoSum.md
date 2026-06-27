# Week 05 — Project 0: Two Sum

## Topic

Project 0 implementation: Two Sum algorithm.

---

## Problem

Given an integer array and a target value, find two different elements whose sum equals the target.

Example:

```text
nums = [2, 7, 11, 15]
target = 9
output = [0, 1]
```

---

## Algorithm Idea

The basic solution is to check every possible pair.

```text
for each i
  for each j
    if nums[i] + nums[j] == target
      return indices
```

---

## Improved Idea

A hash table can improve performance.

For each number:

```text
complement = target - current number
```

If the complement already exists in the hash table, the answer is found.

---

## Complexity

Brute force:

```text
Time: O(n²)
Space: O(1)
```

Hash table:

```text
Time: O(n)
Space: O(n)
```

---

## What I Learned

- How to analyze an algorithm problem.
- How to compare different solutions.
- How to think about time complexity and space complexity.
- How to implement a simple algorithm in C++.

---

## Reflection

Project 0 helped me understand the connection between algorithm design and software engineering. A small problem can still be improved through analysis, testing, and documentation.