# JavaScript: Handling undefined in length checks

This repository demonstrates a common error in JavaScript where attempting to access the 'length' property of an undefined variable leads to an error.  The example showcases the issue and provides a solution.

## Bug

The `foo` function aims to return the length of an array or 0 if the input is null. However, it fails when the input is `undefined` because accessing `undefined.length` throws a TypeError.

## Solution

The solution involves adding a check for `undefined` before accessing the `length` property. This prevents the error and handles all three cases (null, undefined, and array) gracefully.