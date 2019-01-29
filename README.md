# raisinCSS

An Utility CSS only library

## DOCS

### Breakpoints

- `sm`: 576px and up
- `md`: 768px and up
- `lg`: 992px and up
- `xl`: 1200px and up

### Container

Any element with the `.container` class will be centered on screen; with each breakpoint the container goes:

- `sm`: 540px max width;
- `md`: 720px max width;
- `lg`: 960px max width;
- `xl`: 1140px max width;

Using the `.container-fluid` class the element will go 100% width on every screen size.

### CSS Grid

Adding the class `.is-grid` to any element will add the `display:grid` property to it.

We can use grid on each breakpoint adding the prefix:

 `sm:is-grid`
 `md:is-grid`
 `lg:is-grid`
 `xl:is-grid`

By default we are adding `grid-template-columns:auto` and `grid-template-rows:auto` to an `.is-grid` element. For setting the columsn and rows to the grid we can add:

- `.has-{1 to 12}-columns` or
- `.has-{1 to 12}-rows` 

Note: Each columns or row will be `1fr` sized. i.e: 

```html
<div class="is-grid has-12-columns has-4-rows"></div>
```
Will have this css properties:
```css
.my-element {
  display:grid;
  grid-template-columns: repeat(12, 1fr);
  grid-template-rows: repeat(4, 1fr);
}
```


We alse con add the proper breakpoints:

- `.sm:has-{1 to 12}-columns` or
- `.sm:has-{1 to 12}-rows` or
- `.md:has-{1 to 12}-columns` or
- `.md:has-{1 to 12}-rows` and so.

We can also use this classes on an `.is-grid` element:

- `.justify-items-{start | end | center | stretch}`
- `.align-items-{start | end | center | stretch}`
- `.justify-content-{start | end | center | stretch | space-around | space-between | space-evenly}`
- `.align-content-{start | end | center | stretch | space-around | space-between | space-evenly}`
- `.auto-flow-{row | column}`

Also we can add a fixed gap between columns and rows in the grid:

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

- `.from-column-{1 to 12}`
- `.to-column-{1 to 12}`
- `.column-span-{1 to 12}`

- `.from-row-{1 to 12}`
- `.to-row-{1 to 12}`
- `.row-span-{1 to 12}`

Also we can use on any grid item:

- `.justify-self-{start | end | center | stretch}`
- `.align-self-{start | end | center | stretch}`

And of course we can add any breakpoint prefix, i.e:

- `.sm:justify-self-center`
- `.md:align-self-end`

Here an example of a layout grid:
```html
  <div class="container 
    md:is-grid 
    has-12-columns 
    has-4-rows
    column-gap-10 
    lg:column-gap-15 
    row-gap-10 
    justify-grid-items-stretch" style="height:80vh">
    <div class="header 
      from-column-1 
      column-span-12 
      row-span-1" style="background:red; min-height: 100px"></div>
    <div class="main 
      from-column-4 
      to-column-12 
      row-span-2" style="background:green; min-height: 100px"></div>
    <div class="aside 
      from-column-1 
      from-row-2
      column-span-3 
      row-span-2" style="background:blue; min-height: 100px"></div>
    <div class="footer 
      from-column-1 
      to-column-12 
      from-row-4" style="background:yellow; min-height: 100px"></div>
  </div>
```
