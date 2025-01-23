# Unexpected Type Coercion in JavaScript Arithmetic

This repository demonstrates a common error in JavaScript involving unexpected type coercion in arithmetic operations.  The plus (+) operator exhibits different behavior depending on the operands' types. When one operand is a string, it performs string concatenation instead of numerical addition. This can lead to unexpected results if not carefully handled.

## Bug Report
The `bug.js` file contains a function `myFunction` that takes two arguments and returns their sum.  The problem occurs when calling `myFunction` with a number and a string. The expected behavior would be the numerical sum, but instead, string concatenation occurs. 

## Solution
The `bugSolution.js` file provides a solution by explicitly converting the input to numbers using `parseInt()` or `Number()` before the addition operation to ensure numerical addition occurs.
