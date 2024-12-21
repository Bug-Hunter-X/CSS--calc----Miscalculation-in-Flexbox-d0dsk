# CSS `calc()` Miscalculation in Flexbox

This repository demonstrates a common issue with the CSS `calc()` function when used within flexbox layouts.  The problem arises when `calc()` attempts to subtract a pixel value from a percentage-based width or height before the parent container has its dimensions fully determined.  This can lead to unexpected layout results or elements not rendering correctly.

The `bug.css` file contains the buggy code.  The `bugSolution.css` file provides a solution to resolve this issue.

**Problem:** Incorrect or unexpected values are calculated by `calc()` due to the order of layout processing and the dependency on parent container dimensions. 

**Solution:** The solution typically involves ensuring the parent container is properly sized before performing calculations, potentially using techniques such as setting explicit dimensions or utilizing alternative layout strategies.