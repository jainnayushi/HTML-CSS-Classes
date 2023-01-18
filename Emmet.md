># HTML Emmets
```html
div -> <div></div>

div.clss -> <div class="clss"></div>

div#idd -> <div id="#idd"></div>

div.clss#idd -> <div class="clss" id="idd" ></div>

p{This is a para} -> <p>This is a para</p>

Siblings : div+p+h1
<div></div>
<p></p>
<h1></h1>

Nested : nav>ul>li{Item 1}
<nav>
    <ul>
        <li>Item 1</li>
    </ul>
</nav>
Ex : section.main-section>h1.title{My title}+p.body{Text here}
<section class="main-section">
    <h1 class="title">My title</h1>
    <p class="body">body here</p>
</section>

Climb Up : div+div>p>span>em^bq
<div></div>
<div>
    <p>
        <span><em></em></span>
        <blockquote></blockquote>
    </p>
</div>

div+div>p>span>em^^bq
<div></div>
<div>
    <p><span><em></em></span></p>
    <blockquote></blockquote>
</div>

Grouping div+(div>p>span>em)+bq
<div></div>
<div>
    <p><span><em></em></span></p>
</div>
<blockquote></blockquote>

Multiplication 
ul>li 5{Item}
<ul>
    <li>Item</li>
    <li>Item</li>
    <li>Item</li>
    <li>Item</li>
    <li>Item</li>
</ul>
Numbering
ul>li 5{Item $}
<ul>
    <li>Item 1</li>
    <li>Item 2</li>
    <li>Item 3</li>
    <li>Item 4</li>
    <li>Item 5</li>
</ul>

ul>li.item$ 5{Item $}
<ul>
    <li class="item1">Item 1</li>
    <li class="item2">Item 2</li>
    <li class="item3">Item 3</li>
    <li class="item4">Item 4</li>
    <li class="item5">Item 5</li>
</ul>

Numbering start at 3
ul>li.item$@3 5{Item $}
<ul>
    <li class="item3">Item 1</li>
    <li class="item4">Item 2</li>
    <li class="item5">Item 3</li>
    <li class="item6">Item 4</li>
    <li class="item7">Item 5</li>
</ul>

Attributes
p[title="My title"]
<p title="My title"></p>

Implicit
.class
<div class="class"></div>
em>.class
<em><span class="class"></span></em>
ul>.class
<ul>
    <li class="class"></li>
</ul>
```
># CSS Emmets
```css
c#f4
color : #f4f4f4;

p:10
padding:10px;

p:10rem
padding:10rem;

pr:9
padding-right:9px;

t:50
top:50;

w:100%
width:100%;

db
display:block;
di
display:inline;
dib
display:inline-block;
dn
display:none;
df
display:flex;

ff
font-family:serif;
ffa
font-family: Arial, H, H, sans-serif;

fwb
font-weight:bold;
fw700
font-weight:700;

taj
text-align:justify;

fz2em
font-size:20em;

pr15+ml10
padding-right:15px;
margin-left:10px;
