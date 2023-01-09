> # HTML Formatting Elements
* Formatting elements were designed to display special types of text:
```html
<b> - Bold text
<strong> - Important text
<i> - Italic text
<em> - Emphasized text
<mark> - Marked text
<small> - Smaller text
<del> - Deleted text
<ins> - Inserted text
<sub> - Subscript text
<sup> - Superscript text
```

## HTML `<b>` and `<strong>` Elements
* The HTML `<b>` element defines bold text, without any extra importance.
```html
<b>This text is bold</b>
```

* The HTML` <strong>` element defines text with strong importance. The content inside is typically displayed in bold.
```html
<strong>This text is important!</strong>
```

## HTML `<i>` and `<em>` Elements
* The HTML `<i> `element defines a part of text in an alternate voice or mood. The content inside is typically displayed in italic.
* Tip: The `<i>` tag is often used to indicate a technical term, a phrase from another language, a thought, a ship name, etc.
```html
<i>This text is italic</i>
```

* The HTML `<em>` element defines emphasized text. The content inside is typically displayed in italic.
Tip: A screen reader will pronounce the words in `<em>` with an emphasis, using verbal stress.
```html
<em>This text is emphasized</em>
```

> # HTML Quotation and Citation Elements
```html
<abbr> Defines an abbreviation or acronym
<address> Defines contact information for the author/owner of a document
<bdo> Defines the text direction
<blockquote> Defines a section that is quoted from another source
<cite> Defines the title of a work
<q>	Defines a short inline quotation
```
* Example :
```html
<p>WWF's goal is to: <q>Build a future where people live in harmony with nature.</q></p>

<p><cite>The Scream</cite> by Edvard Munch. Painted in 1893.</p>

<blockquote cite="http://www.worldwildlife.org/who/index.html">
For 60 years, WWF has worked to help people and nature thrive. As the world's leading conservation organization, WWF works in nearly 100 countries. At every level, we collaborate with people around the world to develop and deliver innovative solutions that protect communities, wildlife, and the places in which they live.
</blockquote>

<bdo dir="rtl">This line will be written from right to left</bdo>

<address>
Written by John Doe.<br>
Visit us at:<br>
Example.com<br>
Box 564, Disneyland<br>
USA
</address>

<p>The <abbr title="World Health Organization">WHO</abbr> was founded in 1948.</p>
```
> # HTML Comments
* HTML comments are not displayed in the browser, but they can help document your HTML source code.
* You can add comments to your HTML source by using the following syntax:
```html
<!-- Write your comments here -->
```
* Notice that there is an exclamation point (!) in the start tag, but not in the end tag.

># Colors
* HTML colors are specified with predefined color names, or with RGB, HEX, HSL, RGBA, or HSLA values.
```html
<p style="background-color:Tomato;">Lorem ipsum...</p>
```
### RGB- RGBA
* An RGB color value represents RED, GREEN, and BLUE light sources.
* An RGBA color value is an extension of RGB with an Alpha channel (opacity).
* `rgb(red, green, blue)`
* `rgba(red, green, blue, alpha)`
* red,gree,blue - 0 to 255 and alpha - (fully transparent) to 1.0 (not transparent at all)

### HEX
* A hexadecimal color is specified with: #RRGGBB, where the RR (red), GG (green) and BB (blue) hexadecimal integers specify the components of the color
* `#fff000`

### HSL - HSLA
* HSL stands for hue, saturation, and lightness.
* HSLA color values are an extension of HSL with an Alpha channel (opacity).
* `hsl(hue, saturation, lightness)`
* `hsla(hue, saturation, lightness, alpha)`
* Hue is a degree on the color wheel from 0 to 360. 0 is red, 120 is green, and 240 is blue.
* Saturation is a percentage value. 0% means a shade of gray, and 100% is the full color. Saturation can be described as the intensity of a color.
* Lightness is also a percentage value. 0% is black, and 100% is white
* The alpha parameter is a number between 0.0 (fully transparent) and 1.0 (not transparent at all)

> # Images
```html
<img src="img.jpg" alt="Girl's image" width="500" height="600">
```
### Summary

* Use the HTML `<img>` element to define an image
* Use the HTML `src` attribute to define the URL of the image
* Use the HTML `alt` attribute to define an alternate text for an image, if it cannot be displayed
* Use the HTML `width and height` attributes or the CSS width and height properties to define the size of the image

> # Background Image
```css
  background-image: url('img.jpg');
  background-repeat: no-repeat;
  background-attachment: fixed; or cover;
  background-size: 100% 100%;
```

># Lists
1. Unordered List
```html
<ul>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ul>

disc	Sets the list item marker to a bullet (default)
circle	Sets the list item marker to a circle
square	Sets the list item marker to a square
none	The list items will not be marked

<ul style="list-style-type:disc;">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ul>
```
2. Ordered List
```html
<ol>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol>

type="1"	The list items will be numbered with numbers (default)
type="A"	The list items will be numbered with uppercase letters
type="a"	The list items will be numbered with lowercase letters
type="I"	The list items will be numbered with uppercase roman numbers
type="i"	The list items will be numbered with lowercase roman numbers

<ol type="1">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol>
```

3. Description List
* The `<dl>` tag defines the description list, the `<dt> `tag defines the term (name), and the `<dd>` tag describes each term
```html
<dl>
  <dt>Coffee</dt>
  <dd>- black hot drink</dd>
  <dt>Milk</dt>
  <dd>- white cold drink</dd>
</dl>


```
