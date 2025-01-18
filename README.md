# CSS Specificity Bug

This repository demonstrates a common, yet often overlooked, issue in CSS: unexpected behavior due to specificity rules.  The example showcases how combining selectors can lead to styling outcomes that are difficult to predict without a clear understanding of specificity.

## Problem

The primary problem lies in the way CSS resolves conflicting style rules based on selector specificity.  The provided CSS file (`bug.css`) contains conflicting style definitions, resulting in an unexpected color for the element.

## Solution

The solution (`bugSolution.css`) demonstrates how to handle this by either:

1. **Increasing the specificity of the intended style:**  A more specific selector can override conflicting less-specific rules.
2. **Using `!important` (use sparingly):** This can force a style to apply, but is generally considered bad practice because it reduces predictability and makes maintenance more complex.
3. **Re-architecting the CSS:**  Sometimes, restructuring CSS for better organization and reducing conflicts is the ideal solution.  This often involves using more descriptive class names, utilizing the BEM (Block, Element, Modifier) methodology, or adopting other effective CSS methodologies. 

## How to reproduce

1. Clone this repository.
2. Open the HTML file in a web browser. Note the unexpected color.
3. View the provided solution in `bugSolution.css` to understand the different ways the issue can be resolved.