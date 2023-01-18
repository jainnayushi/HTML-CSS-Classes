
># Position
* Static - Default
* Relative  - now we can hve top/bottom/left/right - `Not used this way` since messes upwith document flow
* Absolute - Removes element from doc flow and positions itself in reference to a container - Container should also have a position assigned to it(if not assigned then gets as per html)
* Fixed - Fixed on screen - Never moves even on scroll
* Sticky - fixed + relative - Cannot leave parent container - gets fixed at position assigned - Header
```css
 position: static/relative/fixed/absolute/sticky;
```

<!-- position absolute:child - top 100px - wrt html
position absolute:child + position relative : parent - top 100px - wrt parent -->

># Z-index
* z-index `only works on positioned elements`
* The z-index property specifies the stack order of an element.
```html
<head>
<style>
img {
  position: absolute;
  left: 0px;
  top: 0px;
  z-index: -1;
}
</style>
</head>
<body>

<h1>This is a heading</h1>
<img src="img_tree.png">
<p>Because the image has a z-index of -1, it will be placed behind the text.</p>

</body>
```
div > p

># Combinator Selectors
```html
element element	`div p`	Selects all <p> elements inside <div> elements
element>element	`div > p`	Selects all <p> elements where the parent is a <div> element
element+element	`div + p`	Selects the first <p> element that are placed immediately after <div> elements
element1~element2	`p ~ ul`	Selects every <ul> element that are preceded by a <p> element
```

```html
<head>
<style>
div ~ p {
  background-color: yellow;
}
</style>
</head>
<body>

<h2>General Sibling Selector</h2>

<p>The general sibling selector (~) selects all elements that are next siblings of a specified element.</p>

<p>Paragraph 1.</p>

<div>
  <p>Paragraph 2.</p>
</div>

<p>Paragraph 3.</p>
<code>Some code.</code>
<p>Paragraph 4.</p>

</body>
```

># Pseudo-classes
* A pseudo-class is used to define a special state of an element.
* For example, it can be used to:
- Style an element when a user mouses over it
- Style visited and unvisited links differently
- Style an element when it gets focus
```css
selector:pseudo-class {
  property: value;
}

/* unvisited link */
a:link {
  color: #FF0000;
}

/* visited link */
a:visited {
  color: #00FF00;
}

/* mouse over link */
a:hover {
  color: #FF00FF;
}

/* selected link */
a:active {
  color: #0000FF;
}
```
```html
<head>
<style>
p:first-child {
  color: blue;
} 
</style>
</head>
<body>

<p>This is some text.</p>
<p>This is some text.</p>

<div>
  <p>This is some text.</p>
  <p>This is some text.</p>
</div>

</body>
```
first-child
<div>
 ` <p>p1</p>`
  <p>p1</p>
  <p>p1</p>
  <p>p1</p>
  <p>p1</p>
</div>
<div>
  <h1>heading</h1>
  `<p>p1</p>`
  <p>p1</p>
  <p>p1</p>
  <p>p1</p>
  <p>p1</p>
</div>
<div>
  `<p>p1</p>`
  <p>p1</p>
  <p>p1</p>
  <p>p1</p>
  <p>p1</p>
</div>
># Pseudo-Elements?
* A CSS pseudo-element is used to style specified parts of an element.
* For example, it can be used to:
- Style the first letter, or line, of an element
- Insert content before, or after, the content of an element
* The `::selection `pseudo-element matches the portion of an element that is selected by a user.
- The following CSS properties can be applied to ::selection: color, background, cursor, and outline.
```html
<head>
<style>
p::first-letter {
  color: #ff0000;
  font-size: xx-large;
}
p::first-line {
  color: #0000ff;
  font-variant: small-caps;
}
::selection {
  color: red;
  background: yellow;
}
</style>
</head>
<body>

<p>You can use the ::first-letter pseudo-element to add a special effect to the first character of a text!</p>

</body>

```
># Specificity
* `The selector with the highest specificity value will win and take effect!`
* Every CSS selector has its place in the specificity hierarchy.
* There are four categories which define the specificity level of a selector:
```html
Inline styles - Example: <h1 style="color: pink;">
IDs - Example: #navbar
Classes, pseudo-classes, attribute selectors - Example: .test, :hover, [href]
Elements and pseudo-elements - Example: h1, :before
```
># Calculate Specificity?
* Memorize how to calculate specificity!
* Start at 0,
add 1000 for inline,
 add 100 for each ID value,
  add 10 for each class value (or pseudo-class or attribute selector)
  , add 1 for each element selector or pseudo-element.

Example
```html
A: h1 - 0+1 = 1
B: h1#content = 0+100 + 1 = 101
C: <h1 id="content" style="color: pink;">Heading</h1> = 1000
D: h1.content = 0+10+ 1 = 11


The specificity of A is 1 (one element selector)
The specificity of B is 101 (one ID reference + one element selector)
The specificity of C is 1000 (inline styling)

Since the third rule (C) has the highest specificity value (1000), this style declaration will be applied.
```
># !important?
* The !important rule in CSS is used to add more importance to a property/value than normal.
* In fact, if you use the !important rule, it will override ALL previous styling rules for that specific property on that element!