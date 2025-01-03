# Hack: Stack Overflow in Recursive Factorial Function

This repository demonstrates a common error in Hack: a stack overflow error caused by exceeding the maximum recursion depth in a recursive function.  The `bug.hack` file contains the faulty code, while `bugSolution.hack` provides a corrected version using iteration to avoid the stack overflow.

## Bug Description

The recursive factorial function in `bug.hack` works correctly for small input values. However, for larger inputs (e.g., 50 or higher), it will cause a stack overflow due to excessive recursive calls. This occurs because each recursive call adds a new frame to the call stack, and eventually, the stack's memory limit is exceeded.

## Solution

The `bugSolution.hack` file demonstrates the solution. Instead of recursion, it uses iteration to compute the factorial. This eliminates the unbounded growth of the call stack and avoids the stack overflow error.