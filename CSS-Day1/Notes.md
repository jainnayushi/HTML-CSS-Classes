> # CSS
* Cascading Style Sheets
* The name `cascading` comes from the specified priority scheme to determine which style rule applies if more than one rule matches a particular element. This cascading priority scheme is predictable. The CSS specifications are maintained by the World Wide Web Consortium (W3C).
* CSS describes how HTML elements are to be displayed on screen, paper, or in other media.

># Syntax
* A CSS rule consists of a selector and a declaration block.
```css
selector{
 property : value;
 property : value;
}

h1{
    color:blue;
    font-size:12px;
}
```
># Seletors
* CSS selectors are used to "find" (or select) the HTML elements you want to style.
* We can divide CSS selectors into five categories:

1. Simple selectors (select elements based on name, id, class)
2. Combinator selectors (select elements based on a specific relationship between them)
3. Pseudo-class selectors (select elements based on a certain state)
4. Pseudo-elements selectors (select and style a part of an element)
5. Attribute selectors (select elements based on an attribute or attribute value)

># Id Selector
* The id of an element is unique within a page, so the id selector is used to select one unique element!
* To select an element with a specific id, write a hash (#) character, followed by the id of the element.
```css
#para1 {
  text-align: center;
  color: red;
}
```
># Class Selector
* The class selector selects HTML elements with a specific class attribute.
* To select elements with a specific class, write a period (.) character, followed by the class name.
```css
.center {
  text-align: center;
  color: red;
}
```
># Universal Selector
* The universal selector (*) selects all HTML elements on the page.
```css
* {
  text-align: center;
  color: blue;
}
```
># Grouping Selector
* The grouping selector selects all the HTML elements with the same style definitions.
* Look at the following CSS code (the h1, h2, and p elements have the same style definitions)
* It will be better to group the selectors, to minimize the code.
* To group selectors, separate each selector with a comma.
```css
h1 {
  text-align: center;
  color: red;
}

h2 {
  text-align: center;
  color: red;
}

p {
  text-align: center;
  color: red;
}

h1, h2, p {
  text-align: center;
  color: red;
}
```
># Add CSS
* There are three ways of inserting a style sheet:
1. External CSS
```html
<head>
<link rel="stylesheet" type="text/css" href="mystyle.css">
</head>

<!-- mystyle.css -->
body {
  background-color: linen;
}

h1 {
  color: maroon;
  margin-left: 40px;
}

```
2. Internal CSS
```css
<style>
body {
  background-color: linen;
}

h1 {
  color: maroon;
  margin-left: 40px;
}
</style>
```
3. Inline CSS
```html
<h1 style="color:blue;text-align:center;">This is a heading</h1>
<p style="color:red;">This is a paragraph.</p>
```

>Priority
Inline > Internal > External CSS
># Border
### border-style
```html
dotted - Defines a dotted border
dashed - Defines a dashed border
solid - Defines a solid border
double - Defines a double border
groove - Defines a 3D grooved border. The effect depends on the border-color value
ridge - Defines a 3D ridged border. The effect depends on the border-color value
inset - Defines a 3D inset border. The effect depends on the border-color value
outset - Defines a 3D outset border. The effect depends on the border-color value
none - Defines no border
hidden - Defines a hidden border
```
```css
p.dotted {border-style: dotted;}
p.dashed {border-style: dashed;}
p.solid {border-style: solid;}
p.double {border-style: double;}
p.groove {border-style: groove;}
p.ridge {border-style: ridge;}
p.inset {border-style: inset;}
p.outset {border-style: outset;}
p.none {border-style: none;}
p.hidden {border-style: hidden;}
p.mix {border-style: dotted dashed solid double;}
```
### border-width
```css
p.one {
  border-style: solid;
  border-width: 5px;
}
```
### border-color
```css
p.one {
  border-style: solid;
  border-color: red;
}
```
### border-sides
```css
p {
  border-top-style: dotted;
  border-right-style: solid;
  border-bottom-style: dotted;
  border-left-style: solid;
}
```
1. If the border-style property has four values:
border-style: dotted solid double dashed;
top border is dotted
right border is solid
bottom border is double
left border is dashed

2. If the border-style property has three values:
border-style: dotted solid double;
top border is dotted
right and left borders are solid
bottom border is double

3. If the border-style property has two values:
border-style: dotted solid;
top and bottom borders are dotted
right and left borders are solid

4. If the border-style property has one value:
border-style: dotted;
all four borders are dotted

### Border shorthand
```css
p {
  /* border : width style color */
  border: 5px solid red;
}
```

># Margin
* Margins are used to create space around elements, outside of any defined borders.

* CSS has properties for specifying the margin for each side of an element:
margin-top
margin-right
margin-bottom
margin-left

* All the margin properties can have the following values:
auto - the browser calculates the margin
length - specifies a margin in px, pt, cm, etc.
% - specifies a margin in % of the width of the containing element
inherit - specifies that the margin should be inherited from the parent element

* Negative values are allowed.

1. 4 values - top right bottom left - TRBL - margin: 25px 50px 75px 100px;
2. 3 values - top rightandleft  bottom - T(RL) B - margin: 25px 50px 75px;
3. 2 values - topandbottom rightandleft - (TB)(RL) - margin: 25px 50px;
4. 1 values - all -topandbottomandrightandleft - (TBRL) - margin: 25px;
```css
p {
  margin-top: 100px;
  margin-bottom: 100px;
  margin-right: 150px;
  margin-left: 80px;
}
```
* auto - set the margin property to auto to `horizontally center` the element within its container.
The element will then take up the specified width, and the remaining space will be split equally between the left and right margins.
```css
div {
  width: 300px;
  margin: auto;
  border: 1px solid red;
}
```
* inherit - This example lets the left margin of the <p class="ex1"> element be inherited from the parent element (<div>)
```css
div {
  border: 1px solid red;
  margin-left: 100px;
}

p.ex1 {
  margin-left: inherit;
}
```

># Padding
* Padding is used to create space around an element's content, inside of any defined borders.
* Everything same like margin except `auto is not applicable in padding`