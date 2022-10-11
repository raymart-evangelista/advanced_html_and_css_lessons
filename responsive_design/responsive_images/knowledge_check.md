- What is the main difference between `object-fit` and `background-size`?
  - `object-fit` is meant for `img` tags where you can specify a width and height for images then tell an image how it fits to those dimensions
  - `background-size` don't work on normal `img` tags

- How can you define a width and a height on an `img` without distorting it?
  - if an image is given a flexible width, set the height to `auto`

- Why would you want to provide different images at different screen resolutions?
  - it can be unnecessary to display a large image on a screen significantly smaller than the size it was meant for, can even waste bandwidth for mobile users when an image is intended for desktop users

- When would you want to use an `img` with a `srcset` vs a `picture`?
  - using `srcset` with an `img` to provide several additional source images along with hints to help the browser pick the right one
  - using `<picture>` element can be used to show a smaller portrait image on mobile which zooms in on the person while showing the large landscape shot with a person in the middle when viewed on desktop
  - using `srcset` is for serving differently-sized versions of the same image
  - using `picture` can be used to intentionallyt change the image (art direction)
    - use `picture` when you want both resolution switching and to support multiple image formats