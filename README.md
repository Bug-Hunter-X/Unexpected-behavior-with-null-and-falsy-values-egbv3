# JavaScript Bug: Unexpected Behavior with Null and Falsy Values

This repository demonstrates a common, yet subtle bug in JavaScript related to the handling of null and falsy values.

The `foo` function is intended to add two numbers. It correctly handles `null` inputs by returning `null`. However, it does not handle other falsy values (e.g., `0`, `""`, `false`) correctly.

## Bug

The `bug.js` file contains the buggy code. It returns `null` only when either `a` or `b` is explicitly `null`.  Other falsy values are not treated in the same manner leading to potential unexpected results.

## Solution

The `bugSolution.js` file provides a corrected version of the `foo` function. This version explicitly checks for falsy values, improving the function's robustness.

## How to Run

1. Clone the repository.
2. Open `bug.js` and `bugSolution.js` in a code editor or IDE.
3. Execute the files in your JavaScript environment (e.g., Node.js) to observe the different outputs.

This example highlights the importance of careful handling of null and falsy values in JavaScript and how unexpected behavior can arise from seemingly simple logic.