# Add Two Integers

| Acceptance Rate | Difficulty                                             | Frequency           |
| --------------- | ------------------------------------------------------ | ------------------- |
| 87.7%           | ![Easy](https://img.shields.io/badge/Easy-brightgreen) | ████████████ 76.09% |

## Problem Description

Given two integers `num1` and `num2`, return the sum of the two integers.

## Examples

1. **Input**: `12, 5`  
   **Output**: `17`  
   **Explanation**: `num1` is 12, `num2` is 5, and their sum is `12 + 5 = 17`, so 17 is returned.

2. **Input**: `-10, 4`  
   **Output**: `-6`  
   **Explanation**: `num1 + num2 = -6`, so -6 is returned.

## Constraints

- `-100 <= num1, num2 <= 100`

## Solution

- We are given two values in the argument: `num1` and `num2`.
- The return type must be an `int`, with the sum of values `num1` and `num2`.
- We simply return these two values added together, which will give us the correct result.

### Code

```python
class Solution:
    def sum(self, num1: int, num2: int) -> int:
        return num1 + num2
```
