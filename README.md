# raisinCSS

An Utility CSS only library

### TODO:

- Flex
- Margin and padding
- Border
- Opacity
- Width and height
- text (transforms and decorations)
- Background (positioning, sizing, etc)

## DOCS

### Breakpoints

- `sm`: 576px and up
- `md`: 768px and up
- `lg`: 992px and up
- `xl`: 1200px and up

### Utils

#### Display

We can set the display property as follows:

- `.display-block`
- `.display-inline-block`
- `.display-inline`
- `.display-table`
- `.display-table-row`
- `.display-table-cell`
- `.display-none`

Note: Flex display in a different section

Also we can use the breakpoints prefixes, i.e:

- `.sm:display-none`
- `.md:display-block`
- `.lg:display-inline`
- `.xl:display-table`

#### Float

- `.float-right`
- `.float-left`
- `.float-none`
- `.clearfix`

or:

- `.sm:float-right`
- `.md:float-left`
- `.lg:float-none`
- `.xl:clearfix`

#### Overflow

- `.overflow-auto`
- `.overflow-hidden`
- `.overflow-visible`
- `.overflow-x-auto`
- `.overflow-x-hidden`
- `.overflow-x-visible`
- `.overflow-y-auto`
- `.overflow-y-hidden`
- `.overflow-y-visible`

or:

- `.sm:overflow-auto`
- `.md:overflow-hidden`
- `.lg:overflow-x-none`
- `.xl:overflow-y-scroll`

#### Position

- `.static`
- `.fixed`
- `.absolute`
- `.relative`
- `.sticky`

or:

- `.sm:static`
- `.md:fixed`
- `.lg:absolute`
- `.xl:relative`
- `.md:sticky`

#### Visibility

- `.visible`
- `.hidden`

or:

- `.sm.visible`
- `.md.hidden`

#### Z-index

- `.z-0`
- `.z-10`
- `.z-15`
- `.z-20`
- `.z-25`
- `.z-30`
- `.z-35`
- `.z-40`
- `.z-45`
- `.z-50`
- `.z-auto`

or:

- `.sm:z-0`
- `.md:z-10`
- `.lg:z-25`
- `.xl:z-auto`

#### Font

Setting font-family:

- `.font-sans`
- `.font-serif`
- `.font-mono`

Setting font-style:

- `.font-italic`
- `.font-roman`
- `.font-antialiased`

Setting font-weight:

- `.font-thin` //200
- `.font-light` //300
- `.font-normal` //400
- `.font-medium` //500
- `.font-bold` //700
- `.font-bolder` //800

Setting font-size:

- `.font-xs` //.75rem
- `.font-sm` //.875rem
- `.font-base` //1rem
- `.font-lg` //1.125rem
- `.font-xl` //1.25rem
- `.font-2xl` //1.5rem
- `.font-3xl` //1.875rem
- `.font-4xl` //2.25rem
- `.font-5xl` //3rem

We can use breackpoint prefixes on this classes also (except font-family), i.e:

- `.sm:font-italic`
- `.md:font-thin`
- `.lg:font-xs`
- `.xl:font-bolder`

### Container

Any element with the `.container` class will be centered on screen; with each breakpoint the container goes:

- `sm`: 540px max width;
- `md`: 720px max width;
- `lg`: 960px max width;
- `xl`: 1140px max width;

Using the `.container-fluid` class the element will go 100% width on every screen size.

### CSS Grid

Adding the class `.grid` to any element will add the `display:grid` property to it.

We can use grid on each breakpoint adding the prefix:

 `sm:grid`
 `md:grid`
 `lg:grid`
 `xl:grid`

By default we are adding `grid-template-columns:auto` and `grid-template-rows:auto` to an `.is-grid` element. For setting the columns and rows to the grid we can add:

- `.has-{1 to 12}-columns` or
- `.has-{1 to 12}-rows` 

Note: Each columns or row will be `1fr` sized. i.e: 

```html
<div class="my-element grid has-12-columns has-4-rows"></div>
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

- `.column-start-{1 to 12}`
- `.column-end-{1 to 12}`
- `.column-span-{1 to 12}`

- `.row-start-{1 to 12}`
- `.row-end-{1 to 12}`
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
    md:grid 
    has-12-columns 
    has-4-rows
    column-gap-10 
    lg:column-gap-15 
    row-gap-10 
    justify-items-stretch" style="height:80vh">
    <div class="header 
      column-start-1 
      column-span-12 
      row-span-1" style="background:red; min-height: 100px"></div>
    <div class="main 
      column-start-4 
      column-end-12 
      row-span-2" style="background:green; min-height: 100px"></div>
    <div class="aside 
      column-start-1 
      row-start-2
      column-span-3 
      row-span-2" style="background:blue; min-height: 100px"></div>
    <div class="footer 
      column-start-1 
      column-end-12 
      row-start-4" style="background:yellow; min-height: 100px"></div>
  </div>
```
