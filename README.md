# Problem 1: Distinct Element Sum Algorithm

## Description
This algorithm calculates the sum of all elements that are **distinct** between two sets (arrays). A distinct element is one that appears in **only one of the two sets**.

## Example
Set 1: [3, 1, 7, 9]  
Set 2: [2, 4, 1, 9, 3]  
Common elements: 1, 3, 9  
Distinct elements: 7, 2, 4  
Sum: 13

## Data Structures Used
- Arrays (`set1[]`, `set2[]`)
- Integer variables (`sum`, `i`, `j`)
- A boolean flag (`found`) for checking presence in the other set

## Logic
The algorithm uses **two loops** to:
1. Check all elements in `set1` that do not exist in `set2` and add them to the sum.
2. Then check all elements in `set2` that do not exist in `set1` and also add them to the sum.
This ensures that only **distinct** elements from both sets are included.

## Output
The sum of all distinct elements is printed as the result.


# Problem 2: Dot Product & Orthogonality Check

## Description
This project includes algorithms that:
1. Calculate the dot (scalar) product of two vectors.
2. Use the result to determine if the vectors are orthogonal (dot product = 0).
3. Provide both a procedure-based and function-based version.

## Concepts Covered
- Dot product of vectors
- Orthogonality (dot product = 0)
- Use of arrays to represent vectors
- Nested loops and parameter passing

## Dot Product Formula
Given two vectors:
v1 = [x1, x2, ..., xn]  
v2 = [y1, y2, ..., yn]  

Dot product = x1×y1 + x2×y2 + ... + xn×yn

## Procedure Version
- A procedure named `dot_product` updates a shared variable `ps` by reference.
- It is then used to check orthogonality of multiple vector pairs.

## Function Version
- A function named `dot_product` returns the result directly.
- The main algorithm uses this returned value to check orthogonality.

## Output
For each pair of vectors, the algorithm prints whether they are orthogonal or not.

## Example
Input:  
v1 = [1, 2, 3]  
v2 = [4, -5, 6]  
Dot product = 1×4 + 2×(-5) + 3×6 = 4 -10 + 18 = 12 → Not orthogonal

Input:  
v1 = [1, 2]  
v2 = [-2, 1]  
Dot product = -2 + 2 = 0 → Orthogonal
