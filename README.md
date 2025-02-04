# JavaScript Function with Unexpected NaN

This repository demonstrates a subtle bug in a JavaScript function that leads to unexpected NaN (Not a Number) results when dealing with undefined values.  The function is designed to handle null values gracefully, but it lacks explicit handling for undefined, causing unexpected behavior. 

## Bug Description

The function `foo` intends to return 0 if either argument `a` or `b` is `null`. However, if either argument is `undefined`, the addition operation results in `NaN`, which is not the intended behavior.  The solution below addresses this by explicitly checking for `undefined` using loose comparison. 

## Solution

The solution involves adding a check for `undefined` values in the conditional statement to ensure that the function always returns 0 when either `a` or `b` is `null` or `undefined`.