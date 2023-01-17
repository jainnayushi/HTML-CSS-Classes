># Height, Width and Max-width
* The CSS height and width properties are used to set the height and width of an element.
* The CSS max-width property is used to set the maximum width of an element.

* The height and width properties may have the following values:
1. auto - This is default. The browser calculates the height and width
2. length - Defines the height/width in px, cm, etc.
3. % - Defines the height/width in percent of the containing block
4. initial - Sets the height/width to its default value
5. inherit - The height/width will be inherited from its parent value

># Box Model
* The CSS box model is essentially a box that wraps around every HTML element. It consists of: margins, borders, padding, and the actual content.
* Margin + Border + Padding + Content
```css
div {
  width: 300px;
  border: 15px solid green;
  padding: 50px;
  margin: 20px;
}
```
* The total width of an element should be calculated like this:
* Total element width = `width + left padding + right padding + left border + right border + left margin + right margin`

* The total height of an element should be calculated like this:
* Total element height = `height + top padding + bottom padding + top border + bottom border + top margin + bottom margin`

># Outline
* An outline is a line that is drawn around elements, OUTSIDE the borders, to make the element "stand out".
* CSS has the following outline properties:
1. outline-style
2. outline-color
3. outline-width
4. outline-offset
* The outline-offset property adds space between an outline and the edge/border of an element. The space between an element and its outline is transparent.
```css
p {
  margin: 30px;
  border: 1px solid black;
  outline: 1px solid red;
  outline-offset: 15px;
}
```
### Outline Shorthand
```css
p.ex3 {
  /* outline: width style(req) color */
  outline: 5px solid yellow;
  }
```
DOM Manipulation
># Text
```css
h1{
  color: blue;
  text-align: left/right/center/justify;
  text-align-last: left/right/center/justify;
  direction: rtl;
  unicode-bidi: bidi-override;
  vertical-align: baseline/ text-top/ text-bottom/ sup/ sub

  text-decoration-line : overline/line-through / underline;
  text-decoration-color: red;
  text-decoration-style: dashed;
  text-decoration-thickness: 5px;
  text-decoration: text-decoration-line (required) text-decoration-color (optional) text-decoration-style (optional) text-decoration-thickness (optional)
  text-decoration: underline red double 5px;
  text-decoration: none;

  text-transform: capitalize/lowercase/uppercase

  text-indent: 50px;
  letter-spacing: 5px;
  line-height: 0.8;
  word-spacing: 10px;
  white-space: nowrap;

  text-shadow: hor ver blur color;
  text-shadow: 2px 2px 4px #000000;
}

```
># Fonts
1. Serif fonts have a small stroke at the edges of each letter. They create a sense of formality and elegance.
2. Sans-serif fonts have clean lines (no small strokes attached). They create a modern and minimalistic look.
3. Monospace fonts - here all the letters have the same fixed width. They create a mechanical look. 
4. Cursive fonts imitate human handwriting.
5. Fantasy fonts are decorative/playful fonts.

* In a small-caps font, all lowercase letters are converted to uppercase letters. However, the converted uppercase letters appears in a smaller font size than the original uppercase letters in the text.

```css
font-family: "Times New Roman", Times, serif;
font-style: normal/ italic/oblique;
font-weight: normal/bold;
font-variant: normal/small-caps;
font-size: 40px;
font-size: 2.5em;
font-size: 100%;
font-size:10vw;

font - font-style font-variant font-weight font-size/line-height font-family
font: italic small-caps bold 12px/30px Georgia, serif;
```
* Google fonts


># Units
1. Absolute - px
2. Relative - re,em,vw,vh,%
* % - relative to parent - padding+margin+width
* vw,vh - relative to viewport + padding, margin not counted
* rem - relative to html/root font size - 1 rem=16px;
* rem - relative to html/root font size : Best Choice- Setting - font-size
* em - relative to parent's font size - nested case



