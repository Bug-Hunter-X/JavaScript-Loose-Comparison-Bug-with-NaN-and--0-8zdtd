# JavaScript Loose Comparison Bug

This repository demonstrates a subtle bug in JavaScript's loose comparison (`==`) operator related to `NaN` (Not a Number) and `-0` (negative zero).

## The Bug

JavaScript's loose comparison does not follow the usual rules of equality in some cases. Notably:

* `NaN` is never equal to itself, even using `==`.
* `0` and `-0` are considered equal using `==`.

This behavior can lead to unexpected results in comparisons.

## How to Reproduce

1. Clone this repository.
2. Open `bug.js` and run it in a JavaScript environment (browser console, Node.js, etc.).
3. Observe the unexpected outputs for `NaN` and `-0` comparison using loose equality.