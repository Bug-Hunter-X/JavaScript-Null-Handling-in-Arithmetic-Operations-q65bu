# JavaScript Null Handling Bug

This repository demonstrates a common, yet subtle, bug in JavaScript related to handling null values in arithmetic operations.  The `foo` function attempts to add two numbers, but its handling of null input values could be improved.

## Bug Description

The bug lies in the implicit type coercion that JavaScript performs. When a null value is encountered in an arithmetic operation, it's automatically converted to 0.  While this might seem convenient, it can lead to unexpected behavior and make debugging more difficult, especially in larger codebases where the source of a null value isn't immediately apparent.

## Solution

The provided solution explicitly checks for null values before performing the arithmetic operation and handles them more gracefully and predictably. This enhances the robustness of the function and improves code clarity.