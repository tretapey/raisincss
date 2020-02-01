# Flex

We can use `.flex` to set 'display:flex' on an element. Also, we can set this property on each breakpoint:

- `.sm:flex`
- `.md:flex`
- `.lg:flex`
- `.xl:flex`

We an use this other classes on that element:

## direction

- `.flex-row` -> `flex-direction:row`
- `.flex-column` -> `flex-direction:column`
- `.flex-row-reverse` -> `flex-direction:row-reverse`
- `.flex-column-reverse` -> `flex-direction:column-reverse`

## wraping

- `.flex-wrap`
- `.flex-wrap-reverse`
- `.flex-nowrap`

## justify

- `.justify-start` -> `justify-content: flex-start`
- `.justify-end` -> `justify-content: flex-end`
- `.justify-center` -> `justify-content: center`
- `.justify-between` -> `justify-content: space-between`
- `.justify-around` -> `justify-content: space-around`
- `.justify-evenly` -> `justify-content: space-evenly`

## items align

- `.items-start` -> `align-items: flex-start`
- `.items-end` -> `align-items: flex-end`
- `.items-center` -> `align-items: center`
- `.items-baseline` -> `align-items: baseline`
- `.items-stretch` -> `align-items: stretch`

## content align

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
