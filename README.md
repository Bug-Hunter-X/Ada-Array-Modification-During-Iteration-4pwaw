# Ada Array Modification During Iteration Bug

This repository contains an example of a common error in Ada programming involving array modification during iteration. The bug occurs when attempting to modify array elements within a loop that iterates over the array's range.  If not handled correctly, this can lead to unexpected behavior or runtime errors.

## Bug Description
The `bug.ada` file demonstrates the bug. It iterates through an array and modifies an element. However, this approach can fail if the array is resized or its size is not properly handled during modification.

## Solution
The `bugSolution.ada` file provides a corrected version of the code that solves this issue. The solution involves careful handling of the loop indices to avoid going out of bounds or creating unexpected behavior. 

## How to Reproduce
1. Compile `bug.ada` using an Ada compiler (like GNAT).
2. Run the compiled executable. Observe that unexpected result might occur.
3. Repeat the steps for `bugSolution.ada`. Observe that the result is as intended.

## Lessons Learned
This example highlights the importance of carefully considering how array modification affects iteration loops in Ada. Proper index management is crucial to prevent runtime errors and ensure the code's correctness.