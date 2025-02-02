# CSS calc() Bug: Inaccurate Percentage Calculations

This repository demonstrates a subtle bug in CSS's `calc()` function when dealing with percentages and unresolved parent container widths.  The bug arises when a child element's width (or other property) is calculated as a percentage relative to a parent whose width itself is dependent on percentages or hasn't been resolved yet during the rendering process.

## The Bug
The `bug.css` file contains the CSS code exhibiting the problem.  The issue is that the child element's width is calculated incorrectly because the parent's width is not fully determined at the time of the calculation.

## The Solution
The `bugSolution.css` file provides a solution. This might involve ensuring parent widths are explicitly defined using fixed units (px, em) or using a different calculation approach that avoids percentage dependencies in nested elements.