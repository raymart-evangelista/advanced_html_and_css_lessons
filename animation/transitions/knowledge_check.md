- Are all CSS properties animatable?

- What are the long and short-hand notations for transitions?
  - `transition` property is shorthand for `transition-property`, `transition-duration`, `transition-timing-function`, and `transition-delay`

- What is the stacking context?
  - a stacking context is formed when certain element scenarios are in place such as putting a `transition` property on a `div` element and a `transform` property on the `div` psuedo-class

- Why do you need to keep an eye on repaints?
  - we might end up repainting not only the `div` element, but every element that is stacked on top of it in the stack context