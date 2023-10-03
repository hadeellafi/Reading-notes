# React2

## Conditional Rendering

- used when components will often need to display different things depending on different conditions.
- conditionally render JSX using JavaScript syntax like `if` statements, `&&`, and `? :` operators.

## Rendering Lists

use `filter()` and `map()` with React to filter and transform the array of data into an array of components.

### Keys

Keys tell React which array item each component corresponds to, so that it can match them up later.

#### **Rules of keys**

1. Keys must be unique among siblings.
2. Keys must not change or that defeats their purpose! Don’t generate them while rendering.

## Lifting state

it is when you want the state of two components to always change together.
