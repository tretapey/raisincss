# RaisinCSS

An Utility CSS only library.

- Supports CSS Grid (Check grid section)
- Supports Flexbox
- Totally open to customization
- Skeleton and utility based tool
- Lightweight and easy to use

### Table of contents

- [How to contribute](#how-to-contribute)
- [How to use](#how-to-use)
- [DOCS](#docs)
  - [Breakpoints](#breakpoints)
  - [Utils](#utils)
    - [Display](#display)
    - [Float](#float)
    - [Overflow](#overflow)
    - [Cursor](#cursor)
    - [Position](#position)
    - [Positioning](#positioning)
    - [Visibility](#visibility)
    - [Opacity](#opacity)
    - [Z-index](#z-index)
    - [Margin](#margin)
    - [Padding](#padding)
    - [Width](#width)
    - [Height](#height)
    - [Font](#font)
    - [Text](#text)
    - [Background](#background)
    - [Border](#border)
    - [Shadow](#shadow)
    - [List](#list)
    - [Ratio](#ratio)
  - [Container](#container)
  - [Grid](#grid)
  - [Flex](#flex)
- [Sites using RaisinCSS](#sites-using-raisincss)

## How to contribute

Fork this repo and send a pull request with your proposed changes. Make sure you update docs as well if your changes need to be documented.

To generate the css files run the command `npm install && npm run build` this will generate the following files; `raisin.css`, `raisin.css.map`, `raisin.min.css`, `raisin.min.css.map`.

To generate the css files run the command `yarn && yarn run build` this will generate the following files; `raisin.css`, `raisin.css.map`, `raisin.min.css`, `raisin.min.css.map`.

## How to use

Add this to the `<head>` tag:

```html
<link href="https://cdn.jsdelivr.net/gh/tretapey/raisincss@1.1.0/raisin.min.css" rel="stylesheet"/>
```

or import it in your css:

```css 
@import "https://cdn.jsdelivr.net/gh/tretapey/raisincss@1.1.1/raisin.min.css";
```

or install it via npm:

```npm install raisincss --save``` 

or if you prefer yarn:

```yarn add raisincss```

Also, you can download the file `raisin.min.css` (or an uncompressed version `raisin.css`) directly from this repo and add it manually.

If you want to customize for your own use feel free to fork or download this repo, the `.scss` files has everything you need.

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

Also, we can use the breakpoints prefixes, i.e:

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

#### Cursor

- `.cursor-default`
- `.cursor-grab`
- `.cursor-pointer`
- `.cursor-move`
- `.cursor-not-allowed`
- `.cursor-progress`
- `.cursor-help`
- `.cursor-crosshair`

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

#### Positioning

We can set any positioning property from 0 to 50 with any measure we like as follows:

- `.left-{ 0 | 5 | 10 | 15 | ... | 50 }-{ px | vw | rem | em | vh | % }`
- `.right-{ 0 | 5 | 10 | 15 | ... | 50 }-{ px | vw | rem | em | vh | % }`
- `.top-{ 0 | 5 | 10 | 15 | ... | 50 }-{ px | vw | rem | em | vh | % }`
- `.bottom-{ 0 | 5 | 10 | 15 | ... | 50 }-{ px | vw | rem | em | vh | % }`

or:

- `.sm:left-{ 0 | 5 | 10 | 15 | ... | 50 }-{ px | vw | rem | em | vh | % }`
- `.md:right-{ 0 | 5 | 10 | 15 | ... | 50 }-{ px | vw | rem | em | vh | % }`
- `.lg:top-{ 0 | 5 | 10 | 15 | ... | 50 }-{ px | vw | rem | em | vh | % }`
- `.xl:bottom-{ 0 | 5 | 10 | 15 | ... | 50 }-{ px | vw | rem | em | vh | % }`

If we don't define a measure, then it will use pixels.

#### Visibility

- `.visible`
- `.hidden`

or:

- `.sm.visible`
- `.md.hidden`

#### Opacity

- `.opacity-0` -> `opacity: 0`
- `.opacity-25` -> `opacity: 0.25`
- `.opacity-50` -> `opacity: 0.5`
- `.opacity-75` -> `opacity: 0.75`
- `.opacity-100` -> `opacity: 1`

or:

- `.sm:opacity-0`
- `.md:opacity-75`

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

#### Margin

- `.m-0` -> `margin: 0rem`
- `.m-1` -> `margin: 0.25rem`
- `.m-2` -> `margin: 0.5rem`
- `.m-3` -> `margin: 0.75rem`
- `.m-4` -> `margin: 1rem`
- `.m-5` -> `margin: 1.25rem`
- `.m-6` -> `margin: 1.5rem`
- `.m-7` -> `margin: 1.75rem`
- `.m-8` -> `margin: 2rem`
- `.m-9` -> `margin: 2.25rem`
- `.m-10` -> `margin: 2.5rem`
- `.m-11` -> `margin: 2.75rem`
- `.m-12` -> `margin: 3rem`

We can also use top, right, bottom and left margins:

- `.mt-{0 to 12}` -> `margin-top: {0 to 3}rem`
- `.mr-{0 to 12}` -> `margin-right: {0 to 3}rem`
- `.mb-{0 to 12}` -> `margin-bottom: {0 to 3}rem`
- `.ml-{0 to 12}` -> `margin-left: {0 to 3}rem`
- `.ml-auto`
- `.mr-auto`

Or use the x and y margins:

- `.mx-{0 to 12}`
- `.my-{0 to 12}`
- `.mx-auto`
- `.my-auto`

And we can use any breakpoint prefix, i.e:

- `.sm:m-4`
- `.md:mb-12`
- `.lg:mx-auto`
- `.xl:mr-0`

#### Padding

- `.p-0` -> `padding: 0rem`
- `.p-1` -> `padding: 0.25rem`
- `.p-2` -> `padding: 0.5rem`
- `.p-3` -> `padding: 0.75rem`
- `.p-4` -> `padding: 1rem`
- `.p-5` -> `padding: 1.25rem`
- `.p-6` -> `padding: 1.5rem`
- `.p-7` -> `padding: 1.75rem`
- `.p-8` -> `padding: 2rem`
- `.p-9` -> `padding: 2.25rem`
- `.p-10` -> `padding: 2.5rem`
- `.p-11` -> `padding: 2.75rem`
- `.p-12` -> `padding: 3rem`

We can also use top, right, bottom and left paddings:

- `.pt-{0 to 12}` -> `padding-top: {0 to 3}rem`
- `.pr-{0 to 12}` -> `padding-right: {0 to 3}rem`
- `.pb-{0 to 12}` -> `padding-bottom: {0 to 3}rem`
- `.pl-{0 to 12}` -> `padding-left: {0 to 3}rem`

Or use the x and y paddings:

- `.px-{0 to 12}`
- `.py-{0 to 12}`

And we can use any breakpoint prefix, i.e:

- `.sm:p-4`
- `.md:pb-12`
- `.lg:px-2`
- `.xl:pr-0`

#### Width

- `.w-0` -> `width: 0`
- `.w-1/2` -> `width: 50%`
- `.w-1/3` -> `width: 33.33333%`
- `.w-2/3` -> `width: 66.66667%`
- `.w-1/4` -> `width: 25%`
- `.w-3/4` -> `width: 75%`
- `.w-1/5` -> `width: 20%`
- `.w-2/5` -> `width: 40%`
- `.w-3/5` -> `width: 60%`
- `.w-4/5` -> `width: 80%`
- `.w-1/6` -> `width: 16.66667%`
- `.w-full` -> `width: 100%`
- `.w-screen` -> `width: 100vw`
- `.w-auto` -> `width: auto`

or

- `.sm:w-1/2`
- `.md:w-3/4`
- `.lg:w-full`
- `.xl:w-auto`

#### Height

- `.h-0` -> `height: 0`
- `.h-1/2` -> `height: 50%`
- `.h-1/3` -> `height: 33.33333%`
- `.h-2/3` -> `height: 66.66667%`
- `.h-1/4` -> `height: 25%`
- `.h-3/4` -> `height: 75%`
- `.h-1/5` -> `height: 20%`
- `.h-2/5` -> `height: 40%`
- `.h-3/5` -> `height: 60%`
- `.h-4/5` -> `height: 80%`
- `.h-1/6` -> `height: 16.66667%`
- `.h-full` -> `height: 100%`
- `.h-screen` -> `height: 100vh`
- `.h-auto` -> `height: auto`

or

- `.sm:h-1/2`
- `.md:h-3/4`
- `.lg:h-full`
- `.xl:h-auto`

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

#### Text

- `.text-center`
- `.text-left`
- `.text-right`
- `.text-justify`
- `.text-underline`
- `.text-overline`
- `.text-line-through`
- `.text-capitalize`
- `.text-uppercase`
- `.text-lowercase`

or

- `sm:text-center`
- `md:text-underline`
- `lg:text-uppercase`
- `xl:text-justify`

#### Background

We can set background attachment:

- `.bg-fixed` -> `background-attachment: fixed`
- `.bg-local` -> `background-attachment: local`
- `.bg-scroll` -> `background-attachment: scroll`

Background position:

- `.bg-center`
- `.bg-top`
- `.bg-right`
- `.bg-bottom`
- `.bg-left`
- `.bg-right-top`
- `.bg-right-bottom`
- `.bg-left-top`
- `.bg-left-bottom`

And background repeat:

- `.bg-repeat`
- `.bg-no-repeat`
- `.bg-repeat-x`
- `.bg-repeat-y`

And background size:

- `.bg-auto`
- `.bg-cover`
- `.bg-contain`

And all this classes can be prefixed with a proper breakpoint, i.e:

- `.sm:bg-center`
- `.md:bg-no-repeat`
- `.lg:bg-fixed`
- `.xl:bg-cover`

#### Border

For border property the options are:

- `.border`
- `.border-top`
- `.border-right`
- `.border-bottom`
- `.border-left`
- `.border-solid`
- `.border-dotted`
- `.border-dashed`
- `.border-none`

We can set breakpoints for this classes also:

- `.sm:border`
- `.md:border-top`
- `.lg:border-bottom`
- `.xl:border-none`

By default the border width will be of 1px, we can change that till 6px adding:

- `.border-width-{1 to 6}`

Also, we can change the border radius adding:

- `.border-radius-sm` -> `border-radius: 0.125rem`
- `.border-radius-md` -> `border-radius: 0.25rem`
- `.border-radius-lg` -> `border-radius: 0.5rem`
- `.border-radius-full` -> `border-radius: 50%`
- `.border-radius-pill` -> `border-radius: 50rem`

#### Shadow

The box-shadow property is base on the material design elevation pattern, the values are:

- `.shadow-1`
- `.shadow-2`
- `.shadow-3`
- `.shadow-4`
- `.shadow-5`

We can use breakpoints as well:

- `.sm:shadow-1`
- `.md:shadow-2`
- `.lg:shadow-4`
- `.xl:shadow-5`

#### List

- `.list-unstyled`
- `.list-outside` -> `list-style-position: outside`
- `.list-inside` -> `list-style-position: inside`
- `.list-disc` -> `list-style-type: disc`
- `.list-circle` -> `list-style-type: circle`
- `.list-square` -> `list-style-type: square`
- `.list-decimal` -> `list-style-type: decimal` (1, 2, 3)
- `.list-lower-alpha` -> `list-style-type: lower-alpha` (a, b, c)
- `.list-upper-alpha` -> `list-style-type: upper-alpha` (A, B, C)
- `.list-lower-roman` -> `list-style-type: lower-roman` (i, ii, iii)
- `.list-upper-roman` -> `list-style-type: upper-roman` (I, II, III)

We can use breakpoints:

- `.sm:list-unstyled`
- `.md:list-outside`
- `.lg:list-inside`
- `.xl:list-disc`

#### Ratio

We can add a padding ratio to any element:

- `.ratio-21by9` -> `::before -> padding-top: 42.857143%`
- `.ratio-16by9` -> `::before -> padding-top: 56.25%`
- `.ratio-4by3` -> `::before -> padding-top: 75%`
- `.ratio-1by1` -> `::before -> padding-top: 100%`

### Container

Any element with the `.container` class will be centered on screen; with each breakpoint the container goes:

- `sm`: 540px max width;
- `md`: 720px max width;
- `lg`: 960px max width;
- `xl`: 1140px max width;

Using the `.container-fluid` class the element will go 100% width.

### Grid

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

### Flex

We can use `.flex` to set 'display:flex' on an element. Also, we can set this property on each breakpoint:

- `.sm:flex`
- `.md:flex`
- `.lg:flex`
- `.xl:flex`

We an use this other classes on that element:

##### direction

- `.flex-row` -> `flex-direction:row`
- `.flex-column` -> `flex-direction:column`
- `.flex-row-reverse` -> `flex-direction:row-reverse`
- `.flex-column-reverse` -> `flex-direction:column-reverse`

##### wraping

- `.flex-wrap`
- `.flex-wrap-reverse`
- `.flex-nowrap`

##### justify

- `.justify-start` -> `justify-content: flex-start`
- `.justify-end` -> `justify-content: flex-end`
- `.justify-center` -> `justify-content: center`
- `.justify-between` -> `justify-content: space-between`
- `.justify-around` -> `justify-content: space-around`
- `.justify-evenly` -> `justify-content: space-evenly`

##### items align

- `.items-start` -> `align-items: flex-start`
- `.items-end` -> `align-items: flex-end`
- `.items-center` -> `align-items: center`
- `.items-baseline` -> `align-items: baseline`
- `.items-stretch` -> `align-items: stretch`

##### content align

- `.content-start` -> `align-content: flex-start`
- `.content-end` -> `align-content: flex-end`
- `.content-center` -> `align-content: center`
- `.content-stretch` -> `align-content: stretch`
- `.content-between` -> `align-content: space-between`
- `.content-around` -> `align-content: space-around`

And of course we can use any of this classes with a proper breakpoint prefix, i.e:

- `.sm:justify-start`
- `.md:content-around`
- `.lg:flex-wrap`
- `.xl:items-end`

Items inside `.flex` can use:

- `.self-start` -> `align-self: flex-start`
- `.self-end` -> `align-self: flex-end`
- `.self-center` -> `align-self: center`
- `.self-baseline` -> `align-self: baseline`
- `.self-stretch` -> `align-self: stretch`

And we can use breakpoints prefixes also, i.e:

- `.sm:self-start` -> `align-self: flex-start`
- `.md:self-end` -> `align-self: flex-end`
- `.lg:self-center` -> `align-self: center`
- `.xl:self-baseline` -> `align-self: baseline`


### Sites using RaisinCSS

- [https://cracss.com/](https://cracss.com/) 
- [https://au-dela.ca/](https://au-dela.ca/) 
- [https://www.vengaglobal.com/](https://www.vengaglobal.com/) 
- [https://workday.vengaglobal.com/](https://workday.vengaglobal.com/) 
- [https://edyahn.com/](https://edyahn.com/) 
- [https://raisin.dev/](https://raisin.dev/) 

