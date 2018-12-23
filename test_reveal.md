---
title: test_reveal
theme: white
css: my_custom.css
revealOptions:
    transition: convex
---

# title

## subtitle

those slides are to be used with atom, with the `atom-reveal-md` package

----

If you want to serve the slides outside atom, you need to install the `reveal-md-atomized` package:

```bash
npm install -g reveal-md-atomized
```

Then serve the slides:
```bash
reveal-md test_reveal.md
```

You'll be able to use the presenter view.

---

<!-- .slide: data-background="#00cc66" data-transition="zoom" -->
# Custom slide

- Item 1 <!-- .element: class="fragment" data-fragment-index="2" -->
- Item 2 <!-- .element: class="fragment" data-fragment-index="1" -->


> quote

Note: speaker note to be read in presenter mode (type "S" on keyboard to activate)

---

Top message

## left title <!-- .element: class="left" -->

## right title <!-- .element: class="right" -->

Lorem ipsum blah blah blah <!-- .element: class="left" -->

<img class="right" src="https://via.placeholder.com/500?text=right image">

---

<div>
  <div>
    Top message
  </div>
  <div class="left">
    <h2>Left part</h2>
    With bullet list:
    </br>
    <ul>
      <li> one
      <li> two
      <li> three
    </ul>
  </div>
  <div class="right">
    <h2>Right part</h2>
    <img src="https://via.placeholder.com/200?text=right image">
  </div>
</div>
