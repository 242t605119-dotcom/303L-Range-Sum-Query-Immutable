# LeetCode 303 - Range Sum Query - Immutable

## Problem Statement

Given an integer array `nums`, handle multiple queries to calculate the sum of elements between indices `left` and `right`, including both endpoints.

## Example 1

### Input

```text
nums = [-2, 0, 3, -5, 2, -1]
sumRange(0, 2)
sumRange(2, 5)
sumRange(0, 5)
```

### Output

```text
1
-1
-3
```

## Approach

Use a **Prefix Sum Array**.

The prefix sum stores the sum of all elements up to each position. This allows every range sum to be calculated quickly.

## Algorithm

1. Create a prefix sum array.
2. Store the cumulative sum of the elements.
3. For a query from `left` to `right`, calculate:
   `prefix[right + 1] - prefix[left]`
4. Return the result.

## Time Complexity

* Initialization: `O(n)`
* Each `sumRange` query: `O(1)`

## Space Complexity

`O(n)`

## Key Concepts

* Prefix Sum
* Array
* Range Sum
* Preprocessing

## Language

Python

## LeetCode Details

* **Problem:** 303
* **Title:** Range Sum Query - Immutable
* **Difficulty:** Easy

## Author

**T. Nandhini Reddy**

GitHub: `242t605119-dotcom`
