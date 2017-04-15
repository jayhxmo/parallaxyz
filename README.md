# parallaxyz
Intuitive &amp; Logical Parallax Scrolling for your website — inspired by [Stellar.js](https://github.com/markdalgleish/stellar.js) and [Aristide Benoist](http://www.aristidebenoist.com/).



## Getting Started

Before anything, run 

```
$.parallaxyz();
```

Now, you can add parallax effects to elements on your website.



## Parallax Elements

For now, parallaxyz only supports scroll effects (different scroll speeds of individual elements). Other support coming soon? DM me on [Twitter](https://twitter.com/jayhxmo) if you have any cool suggestions :)

Anyways, to add a scroll speed effect, use

``` html
<element parallaxyz-scroll="value">
```
in your HTML element. Instead of `"value"`, put the value for your desired scroll speed. 1 is the default scroll speed, 2 is 2x the default scroll speed, etc.

So if I wanted my button to scroll 2x faster than other elements, I would do
``` html
<button parallaxy-scroll="2">Scrolls 2x Faster</button>
```

parallaxyz uses the `transform3d` property to add the scroll effects.



## Alignment

By default, elements return to their initial parallax position when they're at the middle of the screen.

So if we had two elements that were vertically aligned (vertically centered to each other) to begin with (different scroll speeds), by default, they would both vertically align when they reach the middle of the screen.

<Insert .gif here of the behavior>

If you don't want this to happen, you can add `parallaxy-align="value"` to the parent / ancestor element
``` html
<div class="parent" parallaxy-align="top">
```
In this example, all the children of this `div` will reach their original position when the `div` reaches the top of the viewport.

Accepted values (for now) are `top`, `center`, `bottom`.



## Questions?

Find me on [Twitter](https://twitter.com/jayhxmo)