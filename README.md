# CSS calc() Unexpected Behavior

This repository demonstrates an unexpected behavior of the `calc()` function in CSS when dealing with percentage values within nested elements.  The `calc()` function does not seem to correctly calculate the width when nested inside an element with a width less than 100% of its parent container.

## Bug Description
The issue occurs when using a percentage value in `calc()` within a nested element. The calculation appears to be performed based on the viewport, not the containing element. 

## Reproduction Steps
1. Clone this repository.
2. Open `index.html` in a web browser. 
3. Observe the width of the inner div. It is smaller than expected.

## Solution
The solution involves explicitly setting the width of the parent element and using absolute units instead of percentages in the nested element's calculation when using `calc()`.