# Grid

Adding the class `.grid` to any element will add the `display:grid` property to it.

We can use grid on each breakpoint adding the prefix:

`sm:grid`
`md:grid`
`lg:grid`
`xl:grid`

By default we are adding `grid-template-columns:auto` and `grid-template-rows:auto` to a `.grid` element. For setting the columns and rows to the grid we can add:

- `.has-{1 to 12}-columns` or
- `.has-{1 to 12}-rows`

Note: Each columns or row will be `1fr` sized. i.e:

```html
<div class="my-element grid has-12-columns has-4-rows"></div>
```

Will have this css properties:

```css
.my-element {
  display: grid;
  grid-template-columns: repeat(12, 1fr);
  grid-template-rows: repeat(4, 1fr);
}
```

We also can add the proper breakpoints:

- `.sm:has-{1 to 12}-columns` or
- `.sm:has-{1 to 12}-rows` or
- `.md:has-{1 to 12}-columns` or
- `.md:has-{1 to 12}-rows` and so.

We can also use this classes on a `.grid` element:

- `.justify-items-{start | end | center | stretch}`
- `.align-items-{start | end | center | stretch}`
- `.justify-content-{start | end | center | stretch | space-around | space-between | space-evenly}`
- `.align-content-{start | end | center | stretch | space-around | space-between | space-evenly}`
- `.auto-flow-{row | column}`

Also, we can add a fixed gap between columns and rows in the grid:

- `.column-gap-{5 | 10 | 15 | 20... | 60}`
- `.row-gap-{5 | 10 | 15 | 20... | 60}`

It will add the number indicated in pixels, i.e: `.column-gap-35` will add a `35px` gap between the grid columns.

Any of this classes listed above can be used with a breakpoint prefix, i.e:

- `.sm:justify-items-center`
- `.md:align-items-center`
- `.lg:justify-content-center`
- `.xl:align-content-center`
- `.md:auto-flow-row`

- `.sm:column-gap-5`
- `.md:row-gap-20`

Any items inside the grid will be auto positioned, we can use this classes on a grid item to change that`:

- `.column-start-{1 to 12}`
- `.column-end-{1 to 12}`
- `.column-span-{1 to 12}`

- `.row-start-{1 to 12}`
- `.row-end-{1 to 12}`
- `.row-span-{1 to 12}`

Also, we can use on any grid item:

- `.justify-self-{start | end | center | stretch}`
- `.align-self-{start | end | center | stretch}`

And we can add any breakpoint prefix, i.e:

- `.sm:justify-self-center`
- `.md:align-self-end`

Here an example of a layout grid:

```html
<div
  class="container 
    md:grid 
    has-12-columns 
    has-4-rows
    column-gap-10 
    lg:column-gap-15 
    row-gap-10 
    justify-items-stretch"
  style="height:80vh"
>
  <div
    class="header 
      column-start-1 
      column-span-12 
      row-span-1"
    style="background:red; min-height: 100px"
  ></div>
  <div
    class="main 
      column-start-4 
      column-end-12 
      row-span-2"
    style="background:green; min-height: 100px"
  ></div>
  <div
    class="aside 
      column-start-1 
      row-start-2
      column-span-3 
      row-span-2"
    style="background:blue; min-height: 100px"
  ></div>
  <div
    class="footer 
      column-start-1 
      column-end-12 
      row-start-4"
    style="background:yellow; min-height: 100px"
  ></div>
</div>
```
