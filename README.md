# Conflicting Hidden Styles in HTML
This example demonstrates a subtle bug that can arise when using both `display: none` and `visibility: hidden` on an HTML element.  While both hide the element, their effects differ, potentially leading to unexpected behavior and layout problems.

## Problem

The `bug.html` file shows an element hidden using both `display: none` and `visibility: hidden`. `display: none` removes the element from the document flow, while `visibility: hidden` makes it invisible but preserves its layout space.  Using both together may not produce the desired result, and can make debugging layout issues difficult.

## Solution

The `solution.html` file demonstrates the solution.  We should only use one method to hide the element consistently.  `display: none` is generally preferred when the element should not affect the page's layout.