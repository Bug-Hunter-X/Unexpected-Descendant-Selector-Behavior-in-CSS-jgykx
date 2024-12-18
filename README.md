# Unexpected Descendant Selector Behavior in CSS

This repository demonstrates a subtle but potentially problematic issue with descendant selectors in CSS. The `bug.css` file contains a CSS rule that unexpectedly applies styles to elements nested deeper than intended due to the nature of descendant selectors. The `bugSolution.css` file provides a corrected approach to achieve the desired styling behavior.

## Bug Description
The issue stems from the use of the descendant selector (.error p) in the CSS rule.  This selector applies styles not only to `<p>` elements directly within elements having the class "error" but also to any nested `<p>` elements. This can lead to unintended styling in complex HTML structures.