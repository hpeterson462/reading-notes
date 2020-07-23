# Canvas Articles

## Basics

* `<canvas>` element
* attributes: width, height
* provide fallback content incase not supported
* canvas starts blank
* `getContext()` method to obtain rendering context and drawing functions

## Drawing Shapes

* grid (coordinate space)
* only supports rectangles and paths - must connect with lines
* filled rectangle: `fillRect(x, y, width, height)` 
* rectangular outline: `strokeRect(x, y, width, height)`
* clears specified rectangle: `clearRect(x, y, width, height)`
* make shapes using paths:
    1) create path
    1) use drawing commands to draw
    1) stroke or fill path to render it
* function that doesn't always draw: `moveTo(xx, y)`
* `for` loop can loop through rows and columns
* Bezier curves - cubic and quadratic varieties


## Applying Styles and Colors

* color = a string representing a CSS color
* `strokeStyle` used to create colored outlines
* transparency - `globalAlpha` property
* line styles and `lineCap` properties
* `miterLimit` and `linejoin` properties
* gradients
* patterns
* shadows 


## Drawing Text

* Two methods: 
    * `fillText(text, x, y [, maxWidth])`
    * `strokeTest(text, x, y [, maxWidth])`
* style text - `textBaseline`
* `measureText()` method to precisely measure text