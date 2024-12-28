# Tailwind CSS justify-between Issue

This repository demonstrates a problem where the Tailwind CSS `justify-between` utility class doesn't function as expected within a flex container. The right-most element fails to align to the far right edge of its parent container.

## Problem

The `justify-between` class is intended to distribute space evenly between flex items and align the first and last items to their respective edges. In this instance, the button (the last item) remains misaligned, defying the expected behavior.

## Solution

The solution involves ensuring that the parent container has sufficient width to accommodate the flex items and the spacing between them. Adding a `w-full` class to the parent ensures it occupies the full available width, resolving the alignment issue.

## Reproduction

1. Clone this repository.
2. Open `bug.html` in a web browser.
3. Observe the misalignment of the button.
4. Open `bugSolution.html` to see the corrected version.