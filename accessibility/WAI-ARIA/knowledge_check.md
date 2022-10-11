- What purpose does WAI-ARIA serve?
  - to define a way to make web content more accessible when native HTML is unable to do so--something that fills in the accessible gaps left by native HTML

- What are the four things ARIA can't do?
  - modify an element's appearance
  - modify an element's behavior
  - add focusability
  - add keyboard event handling

- What are the five rules of ARIA?
  - always use native HTML elements and attributes over ARIA when possible
  - never change native semantics, unless you have no other choice
  - all interactive ARIA controls must be usable with a keyboard
  - never use `role=presentation` or `aria-hidden=true` on focusable elements
  - all interactive elements must have an accessible name

- What is the accessibility tree?
  - contains only the a11y related information that will be used by assistive technologies--ARIA works by modifying properties of the objects that make up this a11y tree

- What are the differences between the three ARIA labels?
  - `aria-labelledby` and `aria-describedby` are two of the ARIA attributes that require another element to be given an `id`
    - `aria-labelledby` attribute overrides both native labels as well as `aria-label` attribute
      - this attribute can have any number of `id` references passed and can also be useful when you want to label an element users of assitive tech, but don't want element's labels to be visible to sighted users (such as in a very minimal shopping website that doesn't visually state the word "Shirts" but can announce the category "Shirts" to users of a11y tech)
    - `aria-describedby` attribute modifies the description property in the a11y tree
      - similar to `aria-labelledby`
      - this attribute modifies the description property in the accessibility tree
  - `aria-label` overrides any native label and modifies the name property in the a11y tree, though it's best used when an elem doesn't already have a native label
    - common use for "close" buttons often seen in menus or modals where instead of the screen reader announcing "X, button", it will announce "close menu, button"

- What does the `aria-hidden` attribute do?
  - hide certain elements, such as decorative images and icons, from the accessibility tree--however the element will remain visible for sighted users
  - all of the children of the element that uses the `aria-hidden` attribute will also become hidden to the a11y tree