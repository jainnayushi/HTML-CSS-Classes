> # Tables
```html
<table>	Defines a table
<th> Defines a header cell in a table
<tr> Defines a row in a table
<td> Defines a cell in a table
<caption> Defines a table caption
<colgroup> Specifies a group of one or more columns in a table for formatting
<thead> Groups the header content in a table
<tbody>	Groups the body content in a table
<tfoot>	Groups the footer content in a table
```
```html
<table>
  <tr>
    <th>Person 1</th>
    <th>Person 2</th>
    <th>Person 3</th>
  </tr>
  <tr>
    <td>Emil</td>
    <td>Tobias</td>
    <td>Linus</td>
  </tr>
  <tr>
    <td>16</td>
    <td>14</td>
    <td>10</td>
  </tr>
</table>
```
### Table Borders
```css
table, th, td {
  border: 1px solid black;
  border-collapse: collapse;
  border-radius: 10px;
  border-color: #96D4D4;
}

dotted     
dashed     
solid     
double     
groove     
ridge     
inset     
outset     
none     
hidden  
```
### Table Sizes
```html
<table style="width:100%">
  <tr>
    <th>Firstname</th>
    <th>Lastname</th>
    <th>Age</th>
  </tr>
  <tr style="height:200px">
    <td>Jill</td>
    <td>Smith</td>
    <td>50</td>
  </tr>
  <tr>
    <td>Eve</td>
    <td>Jackson</td>
    <td>94</td>
  </tr>
</table>
```
### ColSpan and RowSpan
* To make a cell span over multiple rows, use the rowspan attribute
* To make a cell span over multiple columns, use the colspan attribute
```html
<caption>Monthly savings</caption>

<table>
  <tr>
    <th colspan="2">Name</th>
    <th>Age</th>
  </tr>
  <tr>
    <td>Jill</td>
    <td>Smith</td>
    <td>43</td>
  </tr>
  <tr>
    <td>Eve</td>
    <td>Jackson</td>
    <td>57</td>
  </tr>
</table>
```
```html
<table>
  <tr>
    <th>Name</th>
    <td>Jill</td>
  </tr>
  <tr>
    <th rowspan="2">Phone</th>
    <td>555-1234</td>
  </tr>
  <tr>
    <td>555-8745</td>
</tr>
</table>
```
> # Block and Inline
1. Block-level Elements
* A block-level element always `starts on a new line`, and the browsers `automatically add some space` (a margin) before and after the element.

* A block-level element always takes up the `full width` available (stretches out to the left and right as far as it can).

* Two commonly used block elements are: `<p> and <div>`.
* Example : 
```html
<address><article><aside><blockquote><canvas><dd><div><dl><dt><fieldset><figcaption><figure><footer><form><h1>-<h6><header><hr><li><main><nav><noscript><ol><p><pre><section><table><tfoot><ul><video>
```
### `An inline element cannot contain a block-level element!`

2. Inline Elements
* An inline element `does not start on a new line`.
* An inline element only takes up as much `width as necessary`.
* Commonly used : <span>.
* Example : 
```html
<a><abbr><acronym><b><bdo><big><br><button><cite><code><dfn><em><i><img><input><kbd><label><map><object><output><q><samp><script><select><small><span><strong><sub><sup><textarea><time><tt><var>
```


># Semantic Elements
* A semantic element clearly describes its meaning to both the browser and the developer.

* Examples of non-semantic elements: `<div> and <span>` - Tells nothing about its content.

* Examples of semantic elements: `<form>, <table>, and <article>` - Clearly defines its content.

># Form
1. label
2. input
3. type - text
4. type - password
5. type - radio
6. type - checkbox
7. Dropdown
8. Textarea

* for of label should be same as id of input
* name same - radio
* name different - checkbox

```html
    <form>
      <label for="fname">First Name</label>
      <input
        type="text"
        id="fname"
        placeholder="Enter your first name"
      /><br /><br />

      <label for="lname">Last Name</label>
      <input
        type="text"
        id="lname"
        placeholder="Enter your last name"
      /><br /><br />

      <label for="pass">Password</label>
      <input
        type="password"
        id="pass"
        placeholder="Enter your password"
      /><br /><br />
      <p id="a">Checkbox</p>

      <input type="checkbox" id="HTML" name="HTML" />
      <label for="HTML">HTML</label>
      <input type="checkbox" id="CSS" name="CSS" />
      <label for="CSS">CSS</label>
      <input type="checkbox" id="JS" name="JS" />
      <label for="JS">JS</label>

      <br /><br />
      <p>Radio</p>
      <input type="radio" id="HTML" name="lang" />
      <label for="HTML">HTML</label>
      <input type="radio" id="CSS" name="lang" />
      <label for="CSS">CSS</label>
      <input type="radio" id="JS" name="lang" />
      <label for="JS">JS</label>

      <br /><br />
      <label for="Car">Choose a car</label><br>
      <select name="Car" id="cars">
        <option value="volvo">Volvo</option>
        <option value="saab">Saab</option>
        <option value="mercedes">Mercedes</option>
        <option value="audi">Audi</option>
      </select>
      <br /><br />

      <label for="review">Review</label><br>
      <textarea id="review" name="review" rows="4" cols="50">
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Omnis nulla iure ex voluptatem, earum alias perferendis exercitationem dignissimos perspiciatis rerum corporis voluptatibus, eum quibusdam mollitia, facilis voluptate aut vitae aperiam?</textarea>

      <br /><br />
      <button>Submit</button>
```