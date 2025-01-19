# CSS Specificity Bug: Unexpected Color Override

This repository demonstrates a subtle bug related to CSS selector specificity that can lead to unexpected styling issues.  The bug arises from a misunderstanding of how CSS determines which styles to apply when multiple selectors target the same element.

## Bug Description

The bug involves two CSS rules targeting the same element, a paragraph tag. One selector is more specific than the other due to its use of a parent selector leading to an unintended color override. The less specific selector, targeting only the paragraph, should have been expected to dominate, but specificity rules override this.

## How to Reproduce

1. Clone this repository.
2. Open `bug.css` to see the problematic code.
3. Open `bugSolution.css` to see the correction to this issue.
4. Examine the effect in a browser by implementing each CSS file (or view in browser's developer tools).

## Solution

The solution lies in understanding and properly utilizing CSS specificity rules. By carefully choosing and using the more specific selector, or by adjusting the style order of the CSS rules, you can control which styles are applied and avoid unexpected behaviors.

## Additional Notes

This example showcases a scenario that may be overlooked by developers unfamiliar with the nuances of CSS specificity.  Understanding this concept is crucial for preventing unexpected styling issues in more complex CSS projects.