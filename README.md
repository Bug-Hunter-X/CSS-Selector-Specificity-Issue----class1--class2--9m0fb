# CSS Selector Specificity Bug

This repository demonstrates a common CSS issue related to selector specificity. The bug involves an incorrect assumption about the scope of the selector `.class1 .class2`.  The solution explores how to correctly target nested elements.

## Bug
The `bug.css` file contains a CSS rule that only applies to `.class2` elements which are *direct* children of elements with the class `.class1`.  This can lead to styling inconsistencies if you expected the rule to cascade down through nested elements.

## Solution
The `bugSolution.css` file shows how to modify the selector to correctly style all nested instances of `.class2` elements, regardless of their nesting level within `.class1` elements.