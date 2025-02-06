# Inconsistent :focus-visible Pseudo-class Behavior

This repository demonstrates a problem with the `:focus-visible` pseudo-class in CSS.  While it's intended to apply styles only when focus is programmatically triggered, consistent cross-browser behavior isn't guaranteed.

## Problem

The provided CSS styles a button element. When focused using a mouse click or other direct interaction, the button should remain unchanged, but it should change styles when focused programmatically or via tabbing, depending on browser settings and how focus is handled.

However, inconsistencies may appear across different browsers (Chrome, Firefox, Safari, Edge), in how the `:focus-visible` pseudo-class is interpreted and rendered.  This inconsistency can lead to accessibility issues, particularly in applications relying on keyboard navigation.

## Solution (bugSolution.css)

Inconsistent behavior with `:focus-visible` across browsers can be addressed by adopting a polyfill or carefully managing interactions with JavaScript, and potentially providing a fallback focus style.  The solution might involve using JavaScript to detect focus and apply styles accordingly, ensuring a consistent experience across various browsers.