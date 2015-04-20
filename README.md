
# genesass

Smarter defaults + Sass helpers

## About

`genesass` is a collection of (opinionated) default styles and Sass helpers. 

These include:

- Setting the default box-sizing to [border-box](http://paulirish.com/2012/box-sizing-border-box-ftw/).
- [Print styles](https://github.com/aguynamedruchir/genesass/blob/master/core/_print.scss) adapted from [HTML5 Boilerplate](https://github.com/h5bp/html5-boilerplate/blob/master/src/css/main.css).
- Vertical rhythm using [single-direction margins](http://csswizardry.com/2012/06/single-direction-margin-declarations/).
- A [breakpoints map and mixin](https://github.com/aguynamedruchir/genesass/blob/master/core/_responsive-utils.scss) for writing manageable media queries.
- [And lots more!](https://github.com/aguynamedruchir/genesass/blob/master/core/)


## Getting started

Install using `bower` or `npm`
```sh
$ bower install genesass
```

```sh
$ npm install genesass
```

Then, import in your `main.scss` file

```scss
@import "../bower_components/genesass/genesass.scss";
```

```scss
@import "../node_modules/genesass/genesass.scss";
```

It is recommended you include [normalize.css](https://github.com/necolas/normalize.css) before importing `genesass`.


## What's included

`genesass.scss` imports the following files from the `core` folder: 

- **_fixes.scss** Some common fixes, such as setting the box-sizing to border-box and enhancing font rendering.
- **_responsive-utils.scss** A `$breakpoints` map, and a mixin `media-query` to generate media queries from it.
- **_base.scss** Opinionated default styles with configurable variables.
- **_print.scss** Print styles adapted from [HTML5 Boilerplate](https://github.com/h5bp/html5-boilerplate/blob/master/src/css/main.css).


## Configuration

The following variables can be configured for `_base.scss`.

```scss
$color-text: #444;
$color-bg: #fff;
$color-selection: #b3d4fc;

$font-size: 16px;
$sizing-unit: 1rem;
$line-height: 1.625;
$baseline: $line-height * $sizing-unit;
```

A `$breakpoints` map is used for `_responsive-utils.scss`. The default values are based on [Bootstrap's breakpoints](http://getbootstrap.com/css/#responsive-utilities).

```scss
$breakpoints: (
  "xs": "(max-width: 767px)",
  "sm": "(min-width: 768px)",
  "md": "(min-width: 992px)",
  "lg": "(min-width: 1200px)",
  "xl": "(min-width: 1600px)",
);
```


## License

Dedicated to the public domain under [CC0](https://github.com/aguynamedruchir/genesass/blob/master/LICENSE).
