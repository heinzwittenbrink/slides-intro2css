---
title: Grid layouts with frameworks or with CSS grid
author: Heinz Wittenbrink
date: 2017-11-25
---

# Concepts

- Separation of content and layout
- Progressive enhancement


# What is a grid layout?

- Display of content in a number of rows and columns
- 2 dimensions, gutters

---

> Unlike Flexible Box Layout, which is single-axis–oriented, Grid Layout is optimized for 2-dimensional layouts: those in which alignment of content is desired in both dimensions. ([CSS Grid Layout Module Level 1](https://www.w3.org/TR/css-grid-1/ "CSS Grid Layout Module Level 1"))

---

![Exemplary Flex Layout Example](https://www.w3.org/TR/css-grid-1/images/flex-layout.png)

![Exemplary Grid Layout Example]( https://www.w3.org/TR/css-grid-1/images/grid-layout.png)

<p class="copyright" data-fill-with="copyright"><a href="https://www.w3.org/Consortium/Legal/ipr-notice#Copyright">Copyright</a> © 2017 <a href="https://www.w3.org/"><abbr title="World Wide Web Consortium">W3C</abbr></a><sup>®</sup> (<a href="https://www.csail.mit.edu/"><abbr title="Massachusetts Institute of Technology">MIT</abbr></a>, <a href="https://www.ercim.eu/"><abbr title="European Research Consortium for Informatics and Mathematics">ERCIM</abbr></a>, <a href="https://www.keio.ac.jp/">Keio</a>, <a href="http://ev.buaa.edu.cn/">Beihang</a>). W3C <a href="https://www.w3.org/Consortium/Legal/ipr-notice#Legal_Disclaimer">liability</a>, <a href="https://www.w3.org/Consortium/Legal/ipr-notice#W3C_Trademarks">trademark</a> and <a href="http://www.w3.org/Consortium/Legal/2015/copyright-software-and-document">permissive document license</a> rules apply. </p>


---

![](pics/stallman_grid.png){ width=40% }

Rechte: [The CV Inn | Flickr](https://www.flickr.com/photos/the-cv-inn/ "The CV Inn | Flickr") https://creativecommons.org/licenses/by/2.0/


# Responsive grids

- Number and width of columns and rows depend on screen size
- Content has to be flexibly arranged


# Grid Layouts without CSS grid

# Bootstrap as example

- [Grid system · Bootstrap](https://getbootstrap.com/docs/4.0/layout/grid/ "Grid system · Bootstrap")

- Example: [Working With Bootstrap 4 Grid System for Creating Responsive Layouts](https://dzone.com/articles/working-with-bootstrap-4-grid-system-for-creating "Working With Bootstrap 4 Grid System for Creating Responsive Layouts - DZone Mobile")

- [JavaScript · Bootstrap](https://v4-alpha.getbootstrap.com/getting-started/javascript/ "JavaScript · Bootstrap")

# Other grid systems

[9 best grid system for web/mobile UI – Prototypr](https://blog.prototypr.io/9-best-grid-system-for-web-mobile-ui-265c68d30c09 "9 best grid system for web/mobile UI – Prototypr")

# CSS grid

![Five grid items arranged according to content size and available space.](https://www.w3.org/TR/css-grid-1/images/game-smaller.png)

<p class="copyright" data-fill-with="copyright"><a href="https://www.w3.org/Consortium/Legal/ipr-notice#Copyright">Copyright</a> © 2017 <a href="https://www.w3.org/"><abbr title="World Wide Web Consortium">W3C</abbr></a><sup>®</sup> (<a href="https://www.csail.mit.edu/"><abbr title="Massachusetts Institute of Technology">MIT</abbr></a>, <a href="https://www.ercim.eu/"><abbr title="European Research Consortium for Informatics and Mathematics">ERCIM</abbr></a>, <a href="https://www.keio.ac.jp/">Keio</a>, <a href="http://ev.buaa.edu.cn/">Beihang</a>). W3C <a href="https://www.w3.org/Consortium/Legal/ipr-notice#Legal_Disclaimer">liability</a>, <a href="https://www.w3.org/Consortium/Legal/ipr-notice#W3C_Trademarks">trademark</a> and <a href="http://www.w3.org/Consortium/Legal/2015/copyright-software-and-document">permissive document license</a> rules apply. </p>

--- 

![Growth in the grid due to an increase in available space.](https://www.w3.org/TR/css-grid-1/images/game-larger.png)

<p class="copyright" data-fill-with="copyright"><a href="https://www.w3.org/Consortium/Legal/ipr-notice#Copyright">Copyright</a> © 2017 <a href="https://www.w3.org/"><abbr title="World Wide Web Consortium">W3C</abbr></a><sup>®</sup> (<a href="https://www.csail.mit.edu/"><abbr title="Massachusetts Institute of Technology">MIT</abbr></a>, <a href="https://www.ercim.eu/"><abbr title="European Research Consortium for Informatics and Mathematics">ERCIM</abbr></a>, <a href="https://www.keio.ac.jp/">Keio</a>, <a href="http://ev.buaa.edu.cn/">Beihang</a>). W3C <a href="https://www.w3.org/Consortium/Legal/ipr-notice#Legal_Disclaimer">liability</a>, <a href="https://www.w3.org/Consortium/Legal/ipr-notice#W3C_Trademarks">trademark</a> and <a href="http://www.w3.org/Consortium/Legal/2015/copyright-software-and-document">permissive document license</a> rules apply. </p>

---


```html
/**
 * Define the space for each grid item by declaring the grid
 * on the grid container.
 */
#grid {
  /**
   * Two columns:
   *  1. the first sized to content,
   *  2. the second receives the remaining space
   *     (but is never smaller than the minimum size of the board
   *     or the game controls, which occupy this column [Figure 3])
   *
   * Three rows:
   *  3. the first sized to content,
   *  4. the middle row receives the remaining space
   *     (but is never smaller than the minimum height
   *      of the board or stats areas)
   *  5. the last sized to content.
   */
  display: grid;
  grid-template-columns:
    /* 1 */ auto
    /* 2 */ 1fr;
  grid-template-rows:
    /* 3 */ auto
    /* 4 */ 1fr
    /* 5 */ auto;
}

/* Specify the position of each grid item using coordinates on
 * the 'grid-row' and 'grid-column' properties of each grid item.
 */
#title    { grid-column: 1; grid-row: 1; }
#score    { grid-column: 1; grid-row: 3; }
#stats    { grid-column: 1; grid-row: 2; align-self: start; }
#board    { grid-column: 2; grid-row: 1 / span 2; }
#controls { grid-column: 2; grid-row: 3; justify-self: center; }
<div id="grid">
  <div id="title">Game Title</div>
  <div id="score">Score</div>
  <div id="stats">Stats</div>
  <div id="board">Board</div>
  <div id="controls">Controls</div>
</div>

```
[CSS Grid Layout Module Level 1: Adapting Layouts to Available Space](https://www.w3.org/TR/css-grid-1/#adapting-to-available-space "CSS Grid Layout Module Level 1")

# Advantages of CSS grid

# Content:

- Separation of content markup and presentation
- Accessibility

# Design:

- Greater flexibility
- Less dependency on frameworks
- Increased variability

# Code:

- Less code
- Easier code
- Reduced download times


# Progressive enhancement

> Progressive enhancement [starts] ...  by establishing a basic level of user experience that all browsers will be able to provide when rendering your web site, but you also build in more advanced functionality that will automatically be available to browsers that can use it.

---

> At its heart, the progressive enhancement approach prioritises the needs of people, regardless of their technology. Tools, frameworks, and code libraries, on the other hand, are often built to prioritise the needs of designers and developers.

[Resilient Web Design—Chapter 7](https://resilientwebdesign.com/chapter7/ "Resilient Web Design—Chapter 7")
