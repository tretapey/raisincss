# How to use

## CDN

Add this to the `<head>` tag:

```html
<link href="https://cdn.jsdelivr.net/gh/tretapey/raisincss@1.0.4/raisin.min.css" rel="stylesheet"/>
```

or import it in your css:

```css
@import "https://cdn.jsdelivr.net/gh/tretapey/raisincss@1.0.2/raisin.min.css";
```

## NPM Package

or install it via npm:

```npm install raisincss --save``` 

or if you prefer yarn:

```yarn add raisincss```

## Copy file

Also, you can download the file `raisin.min.css` (or an uncompressed version `raisin.css`) directly from this repo and add it manually.

## Add to Sass project

If you want to customize for your own use feel free to fork or download this repo, the `.scss` files has everything you need.

```scss
@import '~raisincss/raisin';
```

If you need to change any of the variables please add changed variables above the import.

Or import each file apon requirements.

```scss
@import 'scss/setup';
@import 'scss/variables';
@import 'scss/display';
@import 'scss/float';
@import 'scss/overflow';
@import 'scss/position';
@import 'scss/visibility';
@import 'scss/opacity';
@import 'scss/z-index';
@import 'scss/margin';
@import 'scss/padding';
@import 'scss/width';
@import 'scss/height';
@import 'scss/font';
@import 'scss/text';
@import 'scss/background';
@import 'scss/border';
@import 'scss/shadow';
@import 'scss/list';
@import 'scss/ratio';
@import 'scss/container';
@import 'scss/grid';
@import 'scss/flex';
@import 'scss/positioning';
```
