- Why should you avoid fixed width?
  - the element will never be able to shrink below that width and can cause issues if the contents of that element run out of room--instead set `max-width`

- Why should you avoid fixed height?
  - child elements inside the fixed height can overflow and run outside of the parent element such as text overflowing from a box--instead set `min-height`
  - in most cases, avoid setting height with some exceptions like headers and footers--but prefer using margin and padding to increase space around content to allow elements flexibility

- In what situations might it be appropriate to use a fixed height or width?
  - keeping a sidebar to always be `250px` or an icon to stay at `32px`

- Why should you avoid percentages?