# Unexpected Layout Behavior with `calc()` in Flexbox

This repository demonstrates a common CSS error related to the usage of the `calc()` function, specifically within a flexbox context.  The problem occurs when `calc()` is used to calculate a width or height, but the parent container does not have its dimensions explicitly set.

## The Bug

The `bug.css` file shows the problematic CSS code. The issue lies in calculating a width based on the parent's width (100%) minus a fixed value (10px). If the parent doesn't have a defined width, the calculation results in unexpected behavior.

## The Solution

The `solution.css` file presents the corrected CSS code.  The solution involves ensuring that the parent container has a defined width (e.g., using `width: 500px;` or `width: 100%;` if the parent is within a fixed-width container) to provide a reliable base for the `calc()` function to operate.