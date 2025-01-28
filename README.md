# JavaScript Null Handling Bug

This repository demonstrates a subtle bug in a JavaScript function that handles null values incorrectly during addition.  The original function returns null if either input is null, regardless of whether the other input is a valid number. The corrected version handles nulls gracefully, treating them as 0 for the addition operation.

## Bug Description
The `foo` function is designed to add two numbers.  However, it returns `null` if either input is `null`, even if the other input is a valid number. This behavior might not be intuitive or expected in all cases.

## Solution
The solution modifies the function to handle null values by treating them as 0 before performing the addition. This ensures that the function works correctly with null or valid number inputs.