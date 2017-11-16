---
title: Introduction to CSS
author: Heinz Wittenbrink
date: 2017-11-16



---

# Remark

---

At this stage most of this presentation is a summary of Rachel Andrews *The New CSS Layout* [-@andrew2017].

![](https://cdn.shopify.com/s/files/1/0051/7692/products/aba-cover-24_100x@3x.png?v=1501539522 "Cover of Andrew's book"){ width=25% }


---

> Don’t just ship the same old layouts with a different underlying technology. Discover what has changed about our medium. Don’t assume that we already know what the web is about to become. [-@andrew2017, p. 7]


# Key concepts

## Separation of content, presentation and behavior

![](https://camo.githubusercontent.com/93685be46ccd43252b02a91c4a086723ae1e5d7b/687474703a2f2f646162316e6d736c76766e74702e636c6f756466726f6e742e6e65742f77702d636f6e74656e742f75706c6f6164732f323031342f30392f313430393732393735366373735f74687265652d6c61796572732e706e67)

## Responsive layouts

![](https://upload.wikimedia.org/wikipedia/commons/1/1f/Responsive-web-design-devices.jpg){ .stretch }

## Progressive enhancement


> Progressive enhancement [starts] ...  by establishing a basic level of user experience that all browsers will be able to provide when rendering your web site, but you also build in more advanced functionality that will automatically be available to browsers that can use it.

---

> At its heart, the progressive enhancement approach prioritises the needs of people, regardless of their technology. Tools, frameworks, and code libraries, on the other hand, are often built to prioritise the needs of designers and developers.

[Resilient Web Design—Chapter 7](https://resilientwebdesign.com/chapter7/ "Resilient Web Design—Chapter 7")


## CSS as a living standard

- Modules
- Continuous development

# Stylesheets with CSS

## CSS as a language for presentation

- Task: presenting marked up content
- Related to channels, devices and context
- Standardized
- Text based

## CSS Grammar

![CSS ruleset](https://developer.mozilla.org/@api/deki/files/6167/=css_syntax_-_ruleset.png)

<small style="font-size: x-small">© [Mozilla Contributors CC-BY-SA 2.5](https://creativecommons.org/licenses/by-sa/2.5/ "Creative Commons — Attribution-ShareAlike 2.5 Generic — CC BY-SA 2.5")</small>

[Syntax - CSS | MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/Syntax "Syntax - CSS | MDN")

## Rules for styling

```css
p {
  color: red;
  font-family: Helvetica, Arial, sans-serif;
}
```

[Fundamental text and font styling - Learn web development | MDN](https://developer.mozilla.org/en-US/docs/Learn/CSS/Styling_text/Fundamentals "Fundamental text and font styling - Learn web development | MDN")

## Typefaces

```html
<head>
  <title>Web Font Sample</title>
  <style type="text/css" media="screen, print">
    @font-face {
      font-family: "Bitstream Vera Serif Bold";
      src: url("http://developer.mozilla.org/@api/deki/files/2934/=VeraSeBd.ttf");
    }
    
    body { font-family: "Bitstream Vera Serif Bold", serif }
  </style>
</head>
<body>
  This is Bitstream Vera Serif Bold.
</body>
</html>
```

[@font-face - CSS | MDN](https://developer.mozilla.org/de/docs/Web/CSS/@font-face "@font-face - CSS | MDN")

## Google fonts

```html
<link href="https://fonts.googleapis.com/css?family=Merriweather" rel="stylesheet">
```
 
 CSS rules to specify these families:

```css
font-family: 'Merriweather', serif;
```

## width and height

- [width - CSS | MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/width "width - CSS | MDN")
- [height - CSS | MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/@media/height "height - CSS | MDN")

## border, margin and padding

[Boxmodell - CSS | MDN](https://developer.mozilla.org/de/docs/Web/CSS/CSS_Boxmodell/Einf%C3%BChrung_in_das_CSS_Boxmodell "Boxmodell - CSS | MDN")

## Other CSS properties

- Short reference: [CSS Properties Reference - CSS | MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Properties_Reference "CSS Properties Reference - CSS | MDN")
- Complete reference (properties, selectors and keywords): [CSS reference - CSS | MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference "CSS reference - CSS | MDN")


# Responsive Design

---

> Responsive design threw everything up in the air again—not only did we need to create designs that used fluid percentage-based  [@andrew2017, p. 11]

---

## Frameworks


# Progressive enhancement

## Progessive enhancement vs. graceful degradation

## HTML and CSS vs. JavaScript

## Complexity and CSS Generation

> The various approaches to CSS architecture—OOCSS ( http://bkaprt.com/ncl/02-01/ ), SMACSS ( http://bkaprt.com/ncl/02-02/ ), BEM ( http://bkaprt.com/ncl /02-03/ ), and so on—may seem like overkill if you are the only person who touches the CSS  [@andrew2017, p. 11]


# Code control

## Developer Tools

## [Codepen](https://codepen.io/)


# Browser compatibility

## Evergreen Browsers

## Tools

> A preprocessor is a tool like Sass ( http://bkaprt.com/ncl/02-04/ ) or LESS ( http://bkaprt.com /ncl/02-05/ ): you write CSS in a language other than CSS, and then compile to CSS. A postprocessor happens after you get to CSS— Autoprefixer ( http://bkaprt.com/ncl/ 02-06/ ) is a good example of such a tool. Autoprefixer runs on your CSS file to add the required additional vendor prefixes for older browsers.  [@andrew2017, p. 11]


---

>	Formal architectures and preprocessors alike have helped enable a trend in web design of breaking things down into smaller components. Brad Frost has described this technique as atomic design ( http://bkaprt.com/ncl/02-07/ ). Pattern library tools such as Pattern Lab ( http://bkaprt.com/ncl/02-08/ ) and Fractal ( http://bkaprt.com/ncl/02-09/ ) provide a framework for working with the hundreds of small components generated by working this way ( Fig 2.1 ). A related concept is that of a style guide or design system ( http://bkaprt. com/ncl/02-10/ ), a document detailing each component, separate from the complete pages that are ultimately generated from thes e pieces . [@andrew2017, p. 20]


## Starting with the content, not with the container
  
>	Such methods encourage us to look at design from the smallest elements outward instead of starting with a blank page and creating a complete design. [@andrew2017, p. 21]


## End of the page paradigm 

> These methods constitute quite a departure from the early days of the web, when we typically thought in “pages” rather than in components.  [@andrew2017, p. 21]

  



	




## Performance as a problem
  
> Another facet of life as a web professional is an increasing focus on performance.


November 13, 2017
	22
	


  

>	The HTTP Archive reported that in December 2016, the average webpage download was over 2.4 MB


November 13, 2017
	22
	
  

> Tim Kadlec’s What Does My Site Cost? ( http://bkaprt.com/ncl/02-15/ ) can give you an appreciation of what it costs people in countries around the world to download you r website.


November 13, 2017
	22
	
  ## CSS and accessability

> Because of their capacity to disconnect the layout from the visual display and keyboard navigation, our newer layout methods also introduce potential accessibility issues.


November 13, 2017
	23
	

	


## Evergreen Browsers


  

> Safari and Edge update with operating system releases;


November 13, 2017
	23
	

	


# Frameworks

---

> Any discussion of modern web design invariably comes around to the fact that all websites look more or less the same. The chief culprit behind these “identikit” websites are frameworks—Bootstrap ( http://bkaprt.com/ncl/02-12/ ) and Foundation ( http://bkaprt.com/ncl/02-13/ ) being key players. These incredibly successful projects enable designers to quickly develop sites with minimal front-end knowledge.  [@andrew2017, p. 21]
  

> But if all your front-end development is in your preferred framework, how long will it be until you can’t remember how to sit down in front of a text editor and build a layout from scratch? How do you find out about new approaches and new specifications? [@andrew2017, p. 25]


# The New Layout



## methods for positioning items in CSS.

- absolute, relative, float

- pre-responsive alternatives

- flexbox

- grid



## CSS Display
  

> The CSS Display specification defines the term formatting context like so: ...the environment into which a set of related boxes are laid out. Different formatting contexts lay out their boxes according to different rules.[@andrew2017, p.26]


	

## Box formatting contexts


> So, given that creating a new BFC to contain floats has become such a frequent requirement, we now have a new value of the display property designed just to create a new BFC: display: flow-root. In browsers that support this new value, it forces a new BFC with no other unwanted effects. [@andrew2017, p.28]

	
## Floated elements and shape outside

> In this version of the specification, and in current browser implementations, you may only use shape-outside on a floated element. [@andrew2017, p.30]

---
> If all goes well, our use of floats as a method for creating multiple-column layouts will fade away. Don’t forget about the humble float, however—you can still include it in your designs. Using CSS Shapes can be a wonderful way to add a little bit of delight to the otherwise straight lines of many designs.  [@andrew2017, p.30]



## relative and absolute positioning
  

> the item that has position: relative on it establishes a new containing block. This becomes helpful when looking at the next value of position, position: absolute.  [@andrew2017, p.31]

> If you decide not to polyfill, then the user will simply not get the nice sticky behavior—the element will remain in flow and scroll with the page. This is a great example of a feature that can be added as a nice enhancement without damaging the experience for users of older browsers. [@andrew2017, p.35]


  
## Multiple-column layouts
  
> Multiple-column layout is a method of splitting up a chunk of content into columns, much as you might see in a newspaper. At first glance, this doesn’t seem to be an appropriate way to display things on the web. But there are good use cases for this specification, [@andrew2017, p.36]



## Multiple column layouts
  

> Multiple-column layout is incredibly simple to use. To split content into three columns, I add the column-count property with a value of the number of columns I would like to have (Fig 3.11). [@andrew2017, p.36]



	


---


  

>	If you add a column-width and a column-count, the column-count will be treated as a maximum number of columns—even if the screen gets wide enough to accommodate more at your requested width.


November 13, 2017
	36
	




  

> This built-in responsiveness is a key part of multiple-column layout, and it was the first specification in which we started to see this kind of behavior.


November 13, 2017
	36
	




  

>	By giving their container a column-width, I can collapse a long list into something that takes up far less room and requires much less scrolling.


November 13, 2017
	37
	

# Flexbox

--- 

>	CSS layout really started to change with the introduction of flexbox, the Flexible Box Module, with features designed for a responsive, flexible web.


November 13, 2017
	37
	

	





  

> All boxes are the same height, even though one box has more content inside.


November 13, 2017
	37
	

	
---



## One-dimensionality 
  

> What happens when flex items wrap onto a new row (or column, if you are working with columns) is that the new row becomes its own flex container.


November 13, 2017
	40
	

> Flexbox won’t try to line the items up with items in rows above or below. We describe this as one-dimensional layout.


November 13, 2017
	40
	

	



## flex-basis, flex-grow and flex-shrink 

> Give the flex item a width; then, in the value of the flex property, set flex-grow and flex-shrink to 0 and flex-basis to auto. Our boxes will not grow from the percentage width, which means that when we only have two items on the row, they do not stretch out and take up all the available space.


November 13, 2017
	40
	

# Grid Layouts
  
---

	CSS Grid Layout does exactly what its name suggests: it enables the creation of grid layouts in CSS. This is two-dimensional layout—laying things out as a row and a column at the same time.


November 13, 2017
	41
	
---

## Defining a grid

[Defining a Grid](https://gridbyexample.com/examples/example1/ "Defining a Grid")



## Line-based placements

[Line-based placement](https://gridbyexample.com/examples/example2/ "Line-based placement")

[Line-based placement shorthand - grid-row and grid-column](https://gridbyexample.com/examples/example3/ "Line-based placement shorthand - grid-row and grid-column")

[Line-based placement shorthand - grid-area](https://gridbyexample.com/examples/example4/ "Line-based placement shorthand - grid-area")

[Line-based placement spanning tracks](https://gridbyexample.com/examples/example5/ "Line-based placement spanning tracks")

[Line-based placement spanning tracks with the span keyword](https://gridbyexample.com/examples/example6/ "Line-based placement spanning tracks with the span keyword")

[Line-based placement named lines](https://gridbyexample.com/examples/example7/ "Line-based placement named lines")

[Line-based placement named lines with spans](https://gridbyexample.com/examples/example8/ "Line-based placement named lines with spans")

## Repeat notation

[Using repeat notation](https://gridbyexample.com/examples/example9/ "Using repeat notation")

## Explicit and implicit grid

[Explicit and Implicit Grid](https://gridbyexample.com/examples/example10/ "Explicit and Implicit Grid")

## Defining grid areas

[Defining Grid Areas](https://gridbyexample.com/examples/example11/ "Defining Grid Areas")


## No clearing required

[No clearing required](https://gridbyexample.com/examples/example12/ "No clearing required")


## Redefining area with media queries

[Redefining Grid Areas with Media Queries](https://gridbyexample.com/examples/example13/ "Redefining Grid Areas with Media Queries")


## Layering items

[Layering items](https://gridbyexample.com/examples/example15/ "Layering items")

## Grid items as positioning context

[A grid item as a new positioning context](https://gridbyexample.com/examples/example16/ "A grid item as a new positioning context")

## Auto-fill

[The auto-fill keyword in repeating track definitions](https://gridbyexample.com/examples/example20/ "The auto-fill keyword in repeating track definitions")

## The minimax-function 

[minmax() in auto-fill repeating tracks](https://gridbyexample.com/examples/example28/ "minmax() in auto-fill repeating tracks")

[minmax() and spanning columns and rows](https://gridbyexample.com/examples/example29/ "minmax() and spanning columns and rows")

[The auto-fill keyword with named grid lines](https://gridbyexample.com/examples/example30/ "The auto-fill keyword with named grid lines")


[A simple minmax example](https://gridbyexample.com/examples/example31/ "A simple minmax example")

---

[Multiple tracks in a track-list with auto-fill](https://gridbyexample.com/examples/example34/ "Multiple tracks in a track-list with auto-fill")



## Auto-fill and auto-fit

[auto-fill vs. auto-fit](https://gridbyexample.com/examples/example37/ "auto-fill vs. auto-fit")

## Aligning the grid

[Aligning the Grid](https://gridbyexample.com/examples/example32/ "Aligning the Grid")

[Aligning the grid with space-around and space-between](https://gridbyexample.com/examples/example33/ "Aligning the grid with space-around and space-between")




## Nested grids

[Nested Grid](https://gridbyexample.com/examples/example21/ "Nested Grid")

## Implicit named grid lines

[Implicit named grid lines](https://gridbyexample.com/examples/example22/ "Implicit named grid lines")

## Order

[Using Order](https://gridbyexample.com/examples/example23/ "Using Order")


---
  

> CSS Grid Layout includes a grid-gap property to space items out. This property is shorthand for grid-column-gap and grid-row-gap, which can also be specified individually.


November 13, 2017
	43
	
[Percentage based grids and gaps](https://gridbyexample.com/examples/example36/ "Percentage based grids and gaps")



---
  

> Just as this book was going to print, the CSS Working Group resolved to change the name of the grid-gap properties. grid-column-gap will become column-gap, grid-row-gap will become row-gap, and the grid-gap shorthand will simply be gap.


November 13, 2017
	43
	
  

> Nothing can rise and land in the grid cell; this differs from the behavior of floats, which try to float up and fill the available space.


November 13, 2017
	45
	

## Named areas
  

> Another method of positioning items on a grid involves using named areas


November 13, 2017
	45


## Empty cells


  

> To leave white space, and to leave a cell empty, use a full-stop character. If you replace the first c with ., that cell will remain empty when the layout is created (Fig 3.21).


November 13, 2017
	47
	
---
  

> keep in mind that although the specification is large and can do a lot of things, it is very simple at its core. You can do a lot with very little CSS.


November 13, 2017
	48
	

# Alignment Control



## The Box Alignment Module
  

>	In Chapter 3, I showed you some examples of flexbox and CSS Grid Layout. These specifications are pulled together by a third specification—the Box Alignment Module Level 3 (http://bkaprt.com/ncl/04-01/).


November 13, 2017
	49
	
## Examples
	
	[Box alignment align-items](https://gridbyexample.com/examples/example24/ "Box alignment align-items")

[Box alignment justify-items](https://gridbyexample.com/examples/example25/ "Box alignment justify-items")

[Box alignment align-self](https://gridbyexample.com/examples/example26/ "Box alignment align-self")

[Box alignment justify-self](https://gridbyexample.com/examples/example27/ "Box alignment justify-self")



---

> Alignment works on items on the cross axis (also known as the block axis in CSS, and as the column axis in the Grid specification). Our flex items are displayed as a row; the cross axis runs across the row vertically, stretching the height of the flex container (Fig 4.4).


November 13, 2017
	51
	

	




## Tools for grid development 
  

> A quick tip: as we start to look at more complex examples, it helps to see the grid defined. Firefox DevTools has a grid highlighter tool (http://bkaprt.com/ncl/04-06/). Inspect the element, then click the little grid icon to see your grid (Fig 4.7).


November 13, 2017
	52
	
## Justification 
  

> The justify-items and justify-self properties do not apply in flexbox because we only have one axis, and the main axis might have multiple items on it.


November 13, 2017
	54  

> The justify-content property acts on


November 13, 2017
	54
	

	





  

> The justify-content property is also the property used to space items out along the main axis. The value space-between creates an equal amount of space between our items; space-around creates an equal amount of space around the items. A third value, space-evenly, distributes the items evenly on the main axis.


November 13, 2017
	55
	


  

> It may seem like overkill to make something a flex item just to center it—and someday we may not need to. The Box Alignment specification details how these alignment properties should work with other layout methods.


November 13, 2017
	56
	



  

> By setting both at once, we have two margins that both want all the space, so the block ends up in the middle. We can apply that to a list of flex items.


November 13, 2017
	59
	
## Writing modes and layout 

  

> In layout, however, the writing mode of the document matters, so with newer layout methods we use logical properties to describe the start edge of our container—wherever that is in terms of the writing mode we are currently in.


November 13, 2017
	60
	

  

> The more I work with flexbox and Grid Layout, the more I find that an understanding of alignment is key to leveraging the power of these specifications.


November 13, 2017
	60
	

	





  

> or remind yourself whether you are aligning content or items this time.


November 13, 2017
	61
	

	





# Responsive by Default


---

> Alignment is just one way in which we see how these modern methods of layout are responsive by default, designed for a world of flexible grids. In this chapter, we’ll look at those flexible grids, and think about how to make the most of the functionality in the specification.


November 13, 2017
	62
	

	

---

> Grid works from the outside in.


November 14, 2017
	64
	  

> define a grid, and then put items into it.


November 14, 2017
	64
	

> To make a grid with a flexible number of columns, we need to create the column listing on the grid container itself; we need to instruct it to “add as many column tracks as will fit.”


November 13, 2017
	64


> What I want to do is to say “as many as will fit” rather than 3, as the first value of repeat(). So instead of using the integer 3, I use the keyword auto-fill (Fig 5.4). For the column-track width, I then need to use an absolute value;


November 13, 2017
	65
	

	





  

> Using minmax() in track sizing enables the setting of a minimum and a maximum size for that track. If we update the 200-pixel track definition to minmax(200px, 1fr), the browser will work out how many 200-pixel columns will fit into the container, and then take the leftover space and assign it equally to the tracks,


November 13, 2017
	66
	

	





  

> The ability to maintain proportions is a key requirement for responsive designs


November 13, 2017
	68
	

	





  

November 13, 2017
	69
	

	




> The key to flexible sizing in flexbox lies in three properties: flex-grow, flex-shrink, and flex-basis. These are applied to the flex items. In Grid, we have the fr unit, which is used when creating track sizes.


November 13, 2017
	68  

> The flex-basis property can be used to set a width (if flex-direction is row) or height (if flex-direction is column) for the flex item.


November 13, 2017
	68

  

> The flex-grow property defines whether an item can grow larger than the size set in flex-basis



  

> The specification advises that authors use the flex shorthand rather than the individual properties of flex-grow, flex-shrink, and flex-basis (http://bkaprt.com/ncl/05-05/).


November 13, 2017
	69
	

	





  

> If I target the first item and change flex-grow on just that item to 2, it grows more than the other two items (Fig 5.10). In this way, the flex properties allow you to scale items in proportion to one another.


November 13, 2017
	70
	

	





  

> A value of content means that the flex-basis is taken from the content size of the item in the main dimension.


November 13, 2017
	70
	

	





  

> If you haven’t set a width, auto resolves to the content size.


November 14, 2017
	71
	

	





  

> I would suggest using auto as your starting point for flex-basis unless you know that you have a specific requirement


November 13, 2017
	71
	

	





  

> there is much value in playing with and testing exactly how the flex properties work; the things that flexbox does that seem mysterious are very much tied up in them.


November 14, 2017
	71
	

	





  

> In CSS Grid Layout, we generally define our proportions when we define our tracks, rather than work from the content out. For this we have the fr unit, which we’ve already met.


November 13, 2017
	71
	

	





  

> In the section about flex-basis, I described how auto works in flexbox, taking the width of the item or resolving to content. In Grid Layout, auto works in roughly the same way; however, be aware that it affects the entire row or column track.


November 13, 2017
	72
	

	





  

> The nice thing about fraction units is that, because they define a fraction of the available space, they can be mixed with tracks set using absolute units.


November 13, 2017
	72
	

	





  

> In the next example, I’ve changed my track listing to create a layout that used to be referred to as the “Holy Grail.” The Holy Grail layout describes fixed-width sidebars and a stretchy middle, with the main content first in the source


November 13, 2017
	72
	

	





  

	


November 13, 2017
	72
	

	





  

> Although allowing rows to auto-size is generally desirable, in some cases, setting columns to auto may result in strange sizing if something in the track affects the widths. Something to keep in mind!


November 13, 2017
	73
	

	





  

> As you can see from this small example, Grid enables the creation of very neat, precise layouts that accommodate the real world of content on the web and the variety of devices we need t


November 14, 2017
	75
	

	





  

> owever, it brings with it a whole new range of potential accessibility issues.


November 14, 2017
	75



# Source Order and Display Order

## Source independence

[Source Independence](https://gridbyexample.com/examples/example14/ "Source Independence")


> This ability to disconnect visual display and source order can be used for good and bad alike; we’ll look at the benefits (and risks) in this chapter.



November 14, 2017
	76
	

	





  

> The flexbox specification includes the property flex-direction, which is how we choose whether to


November 14, 2017
	76
	

	





  

> If you are explicitly placing items on your grid—either by using line-based placement or template areas—you can avoid Grid auto-placing any items


November 14, 2017
	77
	

	





  

> As soon as you create a grid, any direct child flows into that grid—one item per cell.


November 14, 2017
	77
	

	




## grid-auto-flow
  

> Where Grid is most like flexbox is in the grid-auto-flow property. By default, this property is set to row.


November 14, 2017
	77


> Working with Grid auto-placement can almost feel like a completely different layout model again, if your first impression of Grid is a method to define a grid and then state where you want elements to be placed on it.


November 14, 2017
	78
	

	





  

> Many common UI tasks can be achieved with the use of auto-placement, and understanding how it behaves is key to reducing the amount of Grid code you need to write.


November 14, 2017
	78
	

	





  
> We met the grid-auto-flow property earlier in this chapter, when we used it to set the direction of auto-placement to column. This property can also take a keyword of dense or sparse, with sparse the default.


November 14, 2017
	79
	

	





  

> The flexbox and Grid specifications both deal with the issue of accessibility and reordering, and both state that visual reordering does not change the logical order of the document.


November 14, 2017
	80
	

	





  

>	you need to take great care whenever you do something that takes elements away from the order in which they exist in the source


November 14, 2017
	81
	

	





  

	Léonie Watson’s “Flexbox & the keyboard navigation disconnect” (http://bkaprt.com/ncl/06-04/).


November 14, 2017
	81
	

	





  

> and that is to avoid the temptation to flatten out markup to make it easier for elements to become flex or Grid items.


November 14, 2017
	83
	

	





  

>	item only becomes a flex or Grid item if it is a direct child of the flex or Grid container.


November 14, 2017
	83
	

	





  

> Make good decisions for your source and then work out how to manage the visual display of items, even if that requires a little more work at the outset.


November 14, 2017
	83
	

	





  

> only box generation is affected by display: contents.


November 14, 2017
	85
	

	





# Embrace the Future



## Evergreen browsers
  

> how the concept of evergreen browsers is changing the way we think about browser support.


November 14, 2017
	86
	

	





  

> You can import Google Analytics data into caniuse.com (http://bkaprt.com/ncl/07-01/) to see how your data weighs up against global or local data (Fig 7.1).


November 13, 2017
	86
	

	





  

> It’s a good idea to separate out the statistics for mobile devices and desktops. You may find that the mobile devices typically accessing the site have far better support for new features than desktop computers.


November 14, 2017
	87
	

	





  

> you can talk about how modern search engines care about performance and mobile-friendliness. Newer layout methods can assist in making a search-engine-friendly site.


November 13, 2017
	88
	

	





  

> Visitors with older browsers will get a fast and performant website, tailored to the device they have. That’s a far better proposition than trying to somehow create a modern experience using old technology,


November 13, 2017
	89
	

	





  

> 	CSS provides an answer to this question in the shape of feature queries. Feature queries are part of the CSS Conditional Rules Module (http://bkaprt.com/ncl/07-02/), the module that also includes media queries. If you’ve ever used a media query, feature queries will seem very familiar.


November 13, 2017
	89
	

	





  

> That code will be safely tucked away inside your @supports rule, so it won’t be executed by browsers that don’t have support—they won’t understand the rule and therefore will throw


November 14, 2017
	90
	

	




## Feature queries
  

> The approach to take with feature queries is to layer on support in a progressively enhanced way.


November 13, 2017
	90
	

	





  

> that a lot of progressive enhancement involves writing old CSS, then writing the new CSS afterward, exploiting the fact that later CSS will overwrite earlier CSS in your stylesheet.


November 14, 2017
	90
	

	





  

> For both flexbox and Grid, the specification explains that float and clear have no effect on a flex or Grid item. This means that if you float an item, then make it a flex or Grid item, the float will have no effect.


November 13, 2017
	91
	

	





  

> Resetting widths is one of the most common things you will do when creating layouts that work for old and new browsers


November 14, 2017
	93
	

	





  

> a good amount of the overwriting is done simply by dint of the way CSS works, and the additional rules inside feature queries are there only to adjust small things for the supporting browsers.


November 14, 2017
	93
	

	





  

> For this reason, anonymous elements are created. These fix up the DOM tree, ensuring that our cell has a virtual row and table to display inside


November 14, 2017
	94
	

	





  




November 14, 2017
	94
	

	





  

>	then add display: grid to the parent. In a supporting browser, the grid items are blockified, transformed into block elements and not table-cell


November 14, 2017
	95
	

	





  

> Grid makes it very easy to play around with how elements will work at various breakpoints.


November 14, 2017
	96
	

	





# Where are We Going?


---

  

> Brand-new CSS, such as Grid and flexbox, starts life at Level 1 because it never existed in the CSS 2 or 2.1 specifications.


November 14, 2017
	98
	

	





  

> Remember that the CSS Grid Layout specification was in development as a spec and in browsers for well over five years before it became available in production.


November 14, 2017
	98
	

	





  

> Following these discussions is an excellent way to learn more about CSS and how features are implemented in browsers. It quickly gives you an appreciation for the work that goes into creating an interoperable web.


November 14, 2017
	99
	

	





  

> other place where everyone can help move the web forward is in reporting browser bugs and pushing browser vendors to implement features.


November 14, 2017
	99
	

	





  

> If I can leave you with any advice, it is to make room for time to play with new things.


November 14, 2017
	103
	

	





  

> play in an environment like CodePen or JS Bin.


November 14, 2017
	103


