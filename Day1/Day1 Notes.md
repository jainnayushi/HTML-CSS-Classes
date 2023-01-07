> # Introduction
* HTML stands for `Hypertext Markup Language`, and it is the most widely used language to write Web Pages.
* `Hypertext` refers to the way in which Web pages (HTML documents) are linked
together. Thus, the link available on a webpage is called Hypertext.
* As its name suggests, HTML is a `Markup` Language which means you use HTML to
simply "mark-up" a text document with tags that tell a Web browser how to structure
it to display.
# Web Browsers
* The purpose of a web browser (Chrome, Edge, Firefox, Safari) is to read HTML documents and display them correctly.
* A browser does not display the HTML tags, but uses them to determine how to display the document.
# Editor
* Notepad
* VS CODE

<!-- Google - vs code - first link - download - windows - .exe - install - checkbox  -->

> # Basic HTML Document
```html
<!DOCTYPE html>
<html>
<head>
    <title>This is document title</title>
</head>
<body>
    <h1>This is a heading</h1>
    <p>Document content goes here.....</p>
</body>
</html>
```

# Page Structure
* Refer Image

# Case Sensitivity
`HTML is Not Case Sensitive`
* HTML tags are not case sensitive: `<P>` means the same as `<p>`.
* The HTML standard does not require lowercase tags, but W3C recommends lowercase in HTML, and demands lowercase for stricter document types like XHTML.

# The <!DOCTYPE> Declaration
* The <!DOCTYPE> declaration tag is used by the web browser to understand the version of
the HTML used in the document. Current version of HTML is 5 and it makes use of the following declaration:
`<!DOCTYPE html>`
* There are many other declaration types which can be used in HTML document depending on what version of HTML is being used. 

# HEAD - Meta Information
* The `<meta>` tag is used to provide such additional information. * * This tag is an empty element and so does not have a closing tag but it carries information within its attributes
* Can use `<meta>` tag to specify important keywords related to the document and later these keywords are used by the search engines while indexing your webpage for searching
purpose.
```html
<head>
    <title>Title Here</title>
    <!-- <meta name="keywords" content="HTML, Meta Tags, Metadata" /> -->
    <meta name="description" content="Learning about Meta Tags." />
</head>
```
# HTML Element
* An HTML element is defined by a start tag, some content, and an end tag:
`<tagname> Content goes here... </tagname>`
* The HTML element is everything from the start tag to the end tag
* Some doesn't have content and ending tag
```js
<h1>My First Heading</h1>
<p>My first paragraph.</p>
<br>
<hr>
```

# Nested HTML Elements
* HTML elements can be nested (this means that elements can contain other elements).
* All HTML documents consist of nested HTML elements.
* The following example contains four HTML elements (`<html>, <body>, <h1> and <p>`)
---
# HTML Document
* All HTML documents must start with a document type declaration: `<!DOCTYPE html>`.
* The HTML document itself begins with `<html>` and ends with` </html>`.
* The visible part of the HTML document is between `<body>` and `</body>`.

# HTML Headings
* HTML headings are defined with the `<h1> to <h6>` tags.
* `<h1>` defines the most important heading.` <h6>` defines the least important heading: 
```html
<h1>This is heading 1</h1>
<h2>This is heading 2</h2>
<h3>This is heading 3</h3>
```

# HTML Paragraphs
* HTML paragraphs are defined with the `<p>` tag:
```html
<p>This is a paragraph.</p>
```

# HTML Links
* HTML links are defined with the `<a>` tag:
```html
<a href="https://www.google.com">This is a link</a>
```
* The link's destination is specified in the href attribute. 
Attributes are used to provide additional information about HTML elements.

# HTML Images
* HTML images are defined with the <img> tag.
* The source file (src), alternative text (alt), width, and height are provided as attributes:
```html
<img src="Page Structure.png" alt="page structure" width="104" height="142">
```
> # HTML Attributes
* All HTML elements can have attributes
* Attributes provide additional information about elements
* Attributes are always specified in the start tag
* Attributes usually come in name/value pairs like: name="value"

### We Suggest: `Always Quote Attribute Values`
* The HTML standard does not require quotes around attribute values.
However, W3C recommends quotes in HTML, and demands quotes for stricter document types like XHTML.


# Single or Double Quotes?
* Double quotes around attribute values are the most common in HTML, but single quotes can also be used.
* In some situations, when the attribute value itself contains double quotes, it is necessary to use single quotes:
```html
<p title='John "ShotGun" Nelson'>
Or vice versa:
<p title="John 'ShotGun' Nelson">
```
# The href Attribute
* The `<a>` tag defines a hyperlink. The href attribute specifies the URL of the page the link goes to:

```html
<a href="https://www.google.com">Visit W3Schools</a>
```

# The src Attribute
* The <img> tag is used to embed an image in an HTML page. The src attribute specifies the path to the image to be displayed:
```html
<img src="Page Structure.png">
```

* There are two ways to specify the URL in the src attribute:

1. Absolute URL - Links to an external image that is hosted on another website. Example: src="https://www.google.com/images/Page Structure.png".

* Notes: External images might be under copyright. If you do not get permission to use it, you may be in violation of copyright laws. In addition, you cannot control external images; it can suddenly be removed or changed.

2. Relative URL - Links to an image that is hosted within the website. Here, the URL does not include the domain name. If the URL begins without a slash, it will be relative to the current page. Example: src="Page Structure.png". If the URL begins with a slash, it will be relative to the domain. Example: src="/images/Page Structure.png".

* Tip: It is almost always best to use relative URLs. They will not break if you change domain.


# The width and height Attributes
* The `<img>` tag should also contain the width and height attributes, which specify the width and height of the image (in pixels):
```html
<img src="Page Structure.png" width="500" height="600">
```

# The alt Attribute
* The required alt attribute for the `<img>` tag specifies an alternate text for an image, if the image for some reason cannot be displayed. This can be due to a slow connection, or an error in the src attribute, or if the user uses a screen reader.
```html
<img src="Page Structure.png" alt="Girl with a jacket">
```

# The style Attribute
* The style attribute is used to add styles to an element, such as color, font, size, and more.
```html
<p style="color:red;">This is a red paragraph.</p>
```

# The lang Attribute
* You should always include the lang attribute inside the `<html>` tag, to declare the language of the Web page. This is meant to assist search engines and browsers.
* The following example specifies English as the language:
```html
<!DOCTYPE html>
<html lang="en">
<body>
...
</body>
</html>
```

# The title Attribute
* The title attribute defines some extra information about an element.
* The value of the title attribute will be displayed as a tooltip when you mouse over the element:
```html
<p title="I'm a tooltip">This is a paragraph.</p>
```

># Styles

* The HTML style attribute is used to add styles to an element, such as color, font, size, and more.
* The HTML style attribute has the following syntax:
* `<tagname style="property:value;">`
* The property is a CSS property. The value is a CSS value.

# Background Color
* The CSS background-color property defines the background color for an HTML element.
* Set the background color for a page to powderblue:
```html
<body style="background-color:powderblue;">
```

# Text Color
* The CSS color property defines the text color for an HTML element:
```html
<h1 style="color:blue;">This is a heading</h1>
```

# Fonts
* The CSS font-family property defines the font to be used for an HTML element:
```html
<h1 style="font-family:verdana;">This is a heading</h1>
<p style="font-family:courier;">This is a paragraph.</p>
```

# Text Size
* The CSS font-size property defines the text size for an HTML element:
```html
<h1 style="font-size:300%;">This is a heading</h1>
<p style="font-size:160px;">This is a paragraph.</p>
```

# Text Alignment
* The CSS text-align property defines the horizontal text alignment for an HTML element:
```html
<h1 style="text-align:center;">Centered Heading</h1>
<p style="text-align:center;">Centered paragraph.</p>
```

# Summary
* Use background-color for background color
* Use the style attribute for styling HTML elements
* Use color for text colors
* Use font-family for text fonts
* Use font-size for text sizes
* Use text-align for text alignment