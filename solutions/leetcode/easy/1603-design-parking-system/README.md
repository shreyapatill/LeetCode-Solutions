# Add Two Integers

| Acceptance Rate | Difficulty                                             | Frequency           |
| --------------- | ------------------------------------------------------ | ------------------- |
| 88%           | ![Easy](https://img.shields.io/badge/Easy-brightgreen) | n/a |

## Problem Description

You are asked to design a parking system with three types of parking spaces: **big**, **medium**, and **small**. Each type has a fixed number of slots. You need to create a class `ParkingSystem` that:

1. **Initializes** a parking system with the given number of slots for each size (big, medium, small).
2. **Checks** if there is space to add a car of a given type (1 for big, 2 for medium, 3 for small).  
   - If there is at least one empty slot for that car type, park it (decrement the corresponding slot count) and return `true`.
   - Otherwise, return `false`.

## Examples

1. **Example 1**

   - **Input**  
     ```
     ["ParkingSystem", "addCar", "addCar", "addCar", "addCar"]
     [[1, 1, 0], [1], [2], [3], [1]]
     ```
   - **Output**  
     ```
     [null, true, true, false, false]
     ```
   - **Explanation**  
     1. `ParkingSystem(1, 1, 0)` sets up: big = 1, medium = 1, small = 0  
     2. `addCar(1)`: There's 1 big slot, so park the car. Return `true`.  
     3. `addCar(2)`: There's 1 medium slot, so park the car. Return `true`.  
     4. `addCar(3)`: No small slots are available (0), so return `false`.  
     5. `addCar(1)`: The only big slot is already taken, so return `false`.

## Constraints

- `-100 <= num1, num2 <= 100`

## Solution

The approach is very straightforward:
- Maintain a **count** (array or vector) of available slots for each size: `[big, medium, small]`.
- When `addCar(carType)` is called:
  - Check if the available slot count for that car type is greater than 0.
  - If it is, **decrement** the corresponding slot count and return `true`.
  - Otherwise, return `false`.

This logic works in **O(1)** time for each call to `addCar` since it's just a simple check and decrement operation.

### Code


```cpp
#include <vector>

class ParkingSystem {
public:
    std::vector<int> slots;
    
    ParkingSystem(int big, int medium, int small) {
        // slots[0] = big, slots[1] = medium, slots[2] = small
        slots = {big, medium, small};
    }
    
    bool addCar(int carType) {
        // carType - 1 gives index: 0 for big, 1 for medium, 2 for small
        if (slots[carType - 1] > 0) {
            slots[carType - 1]--;
            return true;
        }
        return false;
    }
};
```
## Test Cases

1. **Test Case 1**  
   - **Input**:  
     ```
     ["ParkingSystem","addCar","addCar","addCar","addCar"]
     [[1,1,0],[1],[2],[3],[1]]
     ```
   - **Output**:  
     ```
     [null, true, true, false, false]
     ```

2. **Test Case 2**  
   - **Input**:  
     ```
     ["ParkingSystem","addCar","addCar","addCar"]
     [[0,2,1],[1],[2],[3]]
     ```
     - Explanation: 0 big, 2 medium, 1 small
   - **Output**:  
     ```
     [null, false, true, true]
     ```
     - `addCar(1)` → no big slots → `false`  
     - `addCar(2)` → has medium slots → `true`  
     - `addCar(3)` → has small slot → `true`  

3. **Test Case 3**  
   - **Input**:  
     ```
     ["ParkingSystem","addCar","addCar","addCar","addCar"]
     [[2,2,2],[3],[1],[3],[2]]
     ```
   - **Output**:  
     ```
     [null, true, true, true, true]
     ```
     - Enough slots for all calls.

---

