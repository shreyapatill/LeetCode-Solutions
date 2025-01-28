# One To Ten

| Acceptance Rate | Difficulty                                             |
| --------------- | ------------------------------------------------------ |
| 52%           | ![Easy](https://img.shields.io/badge/Easy-brightgreen) |

## Problem Description

Write a program to print the numbers from **1** through **10**, with each number printed on its own line.

## Constraints

- Execution time limit: 1 second  
- Memory limit: 256 MB 

Since the output is fixed and there is no input, the constraints do not affect the logic.

## Solution

We directly print each number from 1 to 10 using newline characters.

- **Time Complexity**: **O(1)**  
  The program runs in constant time as the output is fixed.
  
- **Space Complexity**: **O(1)**  
  Minimal memory is used for the print statements.


Since the task requires printing a fixed sequence of numbers, using direct output statements with newline separators is the simplest and most efficient method. This avoids unnecessary loops or data structures.

### Code

```cpp
#include <bits/stdc++.h>
using namespace std;

int main() {
  // Prints numbers 1 through 10, each on a new line.
  cout << "1\n2\n3\n4\n5\n6\n7\n8\n9\n10";
  return 0;
}
```

## Test Cases
- **Commands**:
   ```
   g++ work@tech-one-to-ten-beginner.cpp -o one_to_ten
   ./one_to_ten 
   ```
- **Output**:  
  ```
  1
  2
  3
  4
  5
  6
  7
  8
  9
  10
  ```