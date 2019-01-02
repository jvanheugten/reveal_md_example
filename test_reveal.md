---
title: test_reveal
presentation:
  theme: night.css
  showNotes: false
  enableSpeakerNotes: true
---
<!-- @import "my-style.less" -->

<!-- slide -->

# reveal & markdown
## next-gen slides done easily

Those slides are done with [atom](https://atom.io/), with the [markdown-preview-enhanced](https://atom.io/packages/markdown-preview-enhanced) package

<!-- slide -->

Those slides are customized thanks an import statement in the markdown file:
```less
<!-- @import "my-style.less" -->
```

The style file `my-style.less` contains this:
```less
@import url('https://fonts.googleapis.com/css?family=Ubuntu');

.reveal .slides {
    // modify all slides
    font-family: 'Ubuntu', sans-serif;
    h1, h2, h3, h4, h5, h6 {
        font-family: 'Ubuntu', sans-serif;
        text-transform: none;
    }
}
```

<!-- slide -->

If you want to serve the slides outside atom, just export the html file the context menu of the preview with right-click then choose: `HTML > offline`

Then open the HTML file which has been generated with firefox.

If you type `S`, you'll be able to use the presenter view.

<!-- slide vertical=true -->

## Vertical slide

You can have vertically nested slides.

Press escape during presentation to see the slides map.

<!-- .slide:
  data-background="https://opuszine.us/_assets/reviews/my-neighbor-totoro-hayao-miyazaki.jpg"
-->

## Custom slide

You can customize slides properties.

Example: using the `data-background` property:
```
<!-- .slide:
  data-background="https://opuszine.us/_assets/reviews/my-neighbor-totoro-hayao-miyazaki.jpg"
-->
```

<!-- .slide:
  data-background="#4bb"
  data-transition="zoom"
  data-notes="speaker note to be read in presenter mode (type 'S' on keyboard to activate)"
  vertical=true
-->

## Custom slide

Example: using other properties:
```
<!-- .slide:
  data-background="#4bb"
  data-transition="zoom"
  data-notes="speaker note to be read in presenter mode (type 'S' on keyboard to activate)"
-->
```

<!-- slide -->

## Features

Other features are available, like fragments:

- Item 1 <!-- .element: class="fragment" data-fragment-index="2" -->
- Item 2 <!-- .element: class="fragment" data-fragment-index="1" -->

Or quotes:

> Don't believe everything you see on the internet
> [Albert Einstein]

<!-- slide -->

<div>
  Or you can write plain html to use flex & create a 2-columns layout.
</div>
<div style="display:flex">
  <div style="flex:1">
    <h2>Left column</h2>
    With text or bullet list:
    </br>
    <ul>
      <li> one
      <li> two
      <li> three
    </ul>
  </div>
  <div style="flex:1">
    <h2>Right column</h2>
    <img src="https://ichef.bbci.co.uk/news/660/cpsprodpb/025B/production/_85730600_monkey2.jpg">
  </div>
</div>

<!-- slide -->

## Some documentation

https://shd101wyy.github.io/markdown-preview-enhanced/#/presentation
https://github.com/shd101wyy/markdown-preview-enhanced/tree/master/docs
