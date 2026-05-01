# Sum of Distinct Elements Algorithm

## Description
This program calculates the sum of all elements that are **not common** between two arrays (`set1` and `set2`).  
It adds only the elements that appear in one array but not in the other.

---

## Input
- `n`: size of both arrays
- `set1`: first array of size `n`
- `set2`: second array of size `n`

---

## Output
- The sum of all elements that are **distinct (non-common)** between the two arrays.

---

## Algorithm

1. Initialize `sum = 0`
2. Read `n`
3. Read elements of `set1`
4. Read elements of `set2`

### Step 1: Check elements of set1
5. For each element in `set1`:
   - Check if it exists in `set2`
   - If it does NOT exist, add it to `sum`

### Step 2: Check elements of set2
6. For each element in `set2`:
   - Check if it exists in `set1`
   - If it does NOT exist, add it to `sum`

7. Print `sum`

---

## Complexity
- Time Complexity: O(n²)
- Space Complexity: O(1) (excluding input arrays)

---

## Example

### Input
set1 = [1, 2, 3]  
set2 = [3, 4, 5]

### Process
Distinct elements = 1, 2, 4, 5

### Output
sum = 12

---

## Notes
- This is equivalent to finding the **symmetric difference** between two sets and summing it.
