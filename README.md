# Tailwind CSS @apply Directive Error: Non-Existent Utility Class

This repository demonstrates a common error encountered when using Tailwind CSS's `@apply` directive. The error occurs when attempting to apply a utility class that either doesn't exist or has been misspelled within your Tailwind CSS configuration.

## Description

The `@apply` directive is a powerful tool for reusing styles. However, if a class specified using `@apply` does not exist, it will be silently ignored, resulting in unexpected styling behavior, rather than a clear error message.

## How to Reproduce

1.  Clone this repository.
2.  Open `bug.html` in your browser.  Observe that the text is not styled as expected because `text-gray-900` does not exist in the `tailwind.config.js` file.
3.  Open `bugSolution.html` to see the corrected implementation.

## Solution

The solution involves verifying that all utility classes used with `@apply` are correctly defined within your `tailwind.config.js` file (or are included through plugins).  Also, double-check for any typos in class names.