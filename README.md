# Loose Equality and Unexpected NaN in JavaScript

This repository demonstrates a common JavaScript bug related to loose equality (`==`) and its interaction with `null` and `undefined`.  The `foo` function intends to return 0 if the input is null, but produces `NaN` when given `undefined` due to loose equality's behavior.  The solution shows how to use strict equality (`===`) for accurate type checking.

## Bug
The provided `bug.js` file contains the flawed function.  The loose equality (`==`) treats `undefined` and `0` as not equal. 

## Solution
The `bugSolution.js` file demonstrates the corrected function using strict equality (`===`), preventing the `NaN` result. This ensures that only `null` results in a return value of 0.