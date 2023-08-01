# leet-day18

# Readme - Combinations

## Problem Description

Given two integers `n` and `k`, the task is to find all possible combinations of `k` numbers chosen from the range `[1, n]`. The combinations can be returned in any order.

## Examples

### Example 1

Input: `n = 4`, `k = 2`

Output: `[[1,2],[1,3],[1,4],[2,3],[2,4],[3,4]]`

Explanation: There are 4 choose 2 = 6 total combinations. Note that combinations are unordered, i.e., [1,2] and [2,1] are considered to be the same combination.

### Example 2

Input: `n = 1`, `k = 1`

Output: `[[1]]`

Explanation: There is 1 choose 1 = 1 total combination.

## Constraints

- 1 <= n <= 20
- 1 <= k <= n

## Approach and Code

We can solve this problem using backtracking. We define a recursive function called `backtrack` that generates all possible combinations of `k` numbers. The function keeps track of the current combination being formed and adds it to the result vector when its size becomes equal to `k`. The function also maintains a `start` index to avoid repetitions.


## Complexity Analysis

The time complexity of this solution is O(C(n, k) * k) where C(n, k) is the binomial coefficient (n choose k). The space complexity is O(k) for the current vector and O(C(n, k) * k) for the result vector.
