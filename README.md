# Tailwind CSS @apply Bug with Pseudo-elements and content

This repository demonstrates a bug in Tailwind CSS where the `@apply` directive doesn't correctly apply styles to pseudo-elements when the `content` property is involved.  The bug specifically occurs when using `@apply` with directives that modify the `content` property of pseudo-elements such as `:before` or `:after`.

## Bug Description

When applying styles that include the `content` property to pseudo-elements via the `@apply` directive, Tailwind CSS may fail to apply the content correctly. This results in unexpected rendering of pseudo-elements.  The provided example showcases this issue.

## Solution

The proposed solution is to move the `content` style declaration outside of the `@apply` directive. This forces the correct application of the `content` property.

## Steps to Reproduce

1. Clone this repository
2. Open `bug.html` in a web browser. Observe the missing content in the pseudo-element.
3. Open `bugSolution.html` and see the correct application of content.

This is an uncommon bug that usually gets unnoticed, this project serves as a learning opportunity and as a record of a solution to this case.