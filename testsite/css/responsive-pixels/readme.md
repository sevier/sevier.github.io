![Responsive Pixels](https://ind.ie/assets/images/responsive-pixels.svg)

‘Because web development shouldn’t require a calculator.’

# Pixel-perfect responsive design

Responsive pixels is a [Stylus](https://learnboost.github.io/stylus/) library that lets you think in pixels and deploy in rems with pixel fallbacks.

## Think in pixels, deploy in rems.

A responsive pixel is a pixel that is equivalent to one rem. Responsive Pixels achieves this using Stylus mixins. You can scale your whole design up or down by changing the root pixel size on supported browsers (this is exactly how modern browsers scale web sites).

[Read more](http://aralbalkan.com/notes/responsive-pixels/).

## Usage

Clone this repository and import it into your Stylus sytlesheet.

For example, if your project set-up looks like this:

```
my-site
   |__ stylus
         |__ responsive-pixels <— This is where you checked out this project.
         |__ index.styl
```

Then, at the top of *index.styl*, do this to import the library:

```
@import responsive-pixels
```

You can now write your Stylus using only pixel values and they will be translated into the correct REM values with pixel fallbacks. 

For example:

```styl
body
	margin 42px !important
```

Becomes:

```css
body
	margin: 42px !important;
	margin: 2.625rem !important;
```

Enjoy!

## Tests

Run `./test`

**Released with ♥ by [Ind.ie](https://ind.ie) under the MIT License.**