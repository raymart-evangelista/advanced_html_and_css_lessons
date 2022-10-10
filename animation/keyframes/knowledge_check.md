- What are the long and short-hand notations for CSS animations?
  - long-hand notation includes `animation-duration, animation-name, animation-iteration-count, and animation-direction`
  - short-hand notation includes `animation: <animation-duration> <animation-name> <animation-iteration-count> <animation-direction>`

- How do you add keyframes to an animation?
  - reference the animation name, then use `0%`, `100%`, and percentages in between

- When would you use an animation over a transition (and vice versa)?
  - animations when you want to loop a state, don't need a trigger, need something more flexible
  - transitions need a trigger such as pseudo-classes like `:hover` or by adding/removing classes via JS, less flexible, not loopable, changing the opacity of an element when it's active