# genesass

A minimalistic SCSS starter kit.

- `_fixes.scss` Some common fixes, such as setting the box-sizing to border-box and enhancing font rendering.
- `functions.scss` Useful Sass functions.
- `_media-queries.scss` Breakpoints and media queries.
- `_base.scss` Opinionated default styles with customizable variables.
- `_print.scss` Print styles adapted from [HTML5 Boilerplate](https://github.com/h5bp/html5-boilerplate/blob/master/src/css/main.css).


## Getting started

Install using `npm` or `bower`:

```sh
$ npm install --save genesass
```

```sh
$ bower install --save genesass
```

Then, import in your main SCSS file:

```scss
@import "../node_modules/genesass/main/genesass";
```

```scss
@import "../bower_components/genesass/main/genesass";
```

It is recommended you include [normalize.css](https://github.com/necolas/normalize.css) before importing *genesass*.


## Customizing

### \_base.scss

`$line-height` and `$baseline` are used for setting vertical rhythm in `_base.scss`.

```scss
$line-height: 1.625;
$baseline: $line-height * 1rem;
```

### \_media-queries.scss

Breakpoints can be customized for `_media-queries.scss`. The default values are based on [Bootstrap's breakpoints](http://getbootstrap.com/css/#responsive-utilities).

- `xxs`: Watches, wearables
- ` xs`: Phones
- ` sm`: Tablets
- ` md`: Tablets
- ` lg`: Laptops, notebooks
- ` xl`: Desktops (HD)
- `xxl`: Desktops (4K)

```scss
$min-width-xs:   320px;
$min-width-sm:   768px;
$min-width-md:   992px;
$min-width-lg:  1200px;
$min-width-xl:  1920px;
$min-width-xxl: 4096px;
```

Use interpolation to include a media query:

```scss
@media #{$sm} {
  ...
}
```

```scss
@media #{$lg-only} and (orientation: landscape) {
  ...
}
```

```scss
@media #{$xs-only}, #{$sm-only} {
  ...
}
```


## License

Dedicated to the public domain under [CC0](https://github.com/aguynamedruchir/genesass/blob/master/LICENSE).
