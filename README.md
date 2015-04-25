
# genesass

A minimalistic Sass starter kit.

## About

`genesass` is a collection of opinionated default styles and Sass helpers. 

These include:

- Setting the default box-sizing to [border-box](http://paulirish.com/2012/box-sizing-border-box-ftw/).
- [Print styles](https://github.com/aguynamedruchir/genesass/blob/master/main/scss/_print.scss) adapted from [HTML5 Boilerplate](https://github.com/h5bp/html5-boilerplate/blob/master/src/css/main.css).
- Vertical rhythm using [single-direction margins](http://csswizardry.com/2012/06/single-direction-margin-declarations/).
- [Media queries](https://github.com/aguynamedruchir/genesass/blob/master/main/scss/_media-queries.scss) for multi-device development.
- [And lots more!](https://github.com/aguynamedruchir/genesass/blob/master/main/scss/)


## Getting started

Install using `bower` or `npm`
```sh
$ bower install genesass
```

```sh
$ npm install genesass
```

Then import in your main Sass/SCSS file

```scss
@import "../bower_components/genesass/main/genesass";
```

```scss
@import "../node_modules/genesass/main/genesass";
```

It is recommended you include [normalize.css](https://github.com/necolas/normalize.css) before importing `genesass`.


## What's included

`genesass` includes: 

- **_fixes.scss** Some common fixes, such as setting the box-sizing to border-box and enhancing font rendering.
- **_media-queries.scss** Breakpoint and media query variables.
- **_base.scss** Opinionated default styles with customizable variables.
- **_print.scss** Print styles adapted from [HTML5 Boilerplate](https://github.com/h5bp/html5-boilerplate/blob/master/src/css/main.css).


## Customizing

The following variables can be configured for `_base.scss`.

```scss
$color-text: #333;
$color-bg: #fff;
$color-selection: #b3d4fc;

$font-size: 16px;

$line-height: 1.625;
$baseline: $line-height * 1rem;
```

Breakpoints can be configured for `_media-queries.scss`. The default values are based on [Bootstrap's breakpoints](http://getbootstrap.com/css/#responsive-utilities).

```scss
$breakpoint-sm:  768px;
$breakpoint-md:  992px;
$breakpoint-lg: 1200px;
$breakpoint-xl: 1600px;
```


## License

Dedicated to the public domain under [CC0](https://github.com/aguynamedruchir/genesass/blob/master/LICENSE).
