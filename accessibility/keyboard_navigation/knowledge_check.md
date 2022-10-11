- What are two things that interactive elements must have for keyboard users?
  - focusable and event handle-able

- What are focus styles?
  - outline or border surrounding the element when it receives focus

- Why should you never completely remove focus styles from an element?
  - it can make it impossible for keyboard users to navigate and operate as they have no visual indication what element actually has focus

- What is the tab order?
  - order in which elements on the page will receive focus when pressing the Tab key

- What is the best way to hide hidden content from assistive technologies?
  - give hidden content a `tabindex` value of -1 or giving the container for the hidden content itself either `display: none` or `visibility: none` CSS property when it's hidden--this removes the menu items from tab order and prevents assistive tech from announcing them