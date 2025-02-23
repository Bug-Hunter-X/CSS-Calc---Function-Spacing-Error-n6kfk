# CSS Calc() Spacing Bug

This repository demonstrates a common, yet easily overlooked, error in CSS: incorrect spacing within the `calc()` function.  Forgetting to include spaces around the operators (+, -, 
*, /) can lead to unexpected behavior and layout issues.

The `bug.css` file contains the erroneous code, while `bugSolution.css` provides the corrected version.  The readme explains the problem and solution in detail.

## Problem
The `calc()` function in CSS is a powerful tool for performing calculations.  However, it's crucial to use spaces correctly around operators.  Failure to do so can lead to the browser misinterpreting the calculation and producing unintended results.  The browser might not be able to parse the expression correctly, causing the calculation to fail.

## Solution
The solution is simple: ensure that you always include spaces before and after the operators within the `calc()` function. This makes the calculation unambiguous and allows the browser to parse it correctly.

## Example

**Incorrect:**
```css
width:calc(100%-10px);
```

**Correct:**
```css
width:calc(100% - 10px);
```