[TOC]
<!-- @import "[TOC]" {cmd="toc" depthFrom=1 depthTo=6 orderedList=false} -->

<!-- code_chunk_output -->

- [HTML](#html)
- [Editors](#editors)
- [Basic Strucutre of HTML](#basic-structure-of-html)
- [Extension](#extension)
- [HTML Elements && Attributes](#html-elements--attributes)
- [Block Level vs Inline](#block-level-vs-inline)
- [To View HTML Source from Browser](#to-view-html-source-from-browser)
- [Different Tags](#different-tags)
  - [Headings](#headings)
  - [Paragraph](#paragraph)
  - [Styles](#styles)
  - [Formatting](#formatting)
  - [Quotation Tags](#quotation-tags)
  - [Colors](#colors)
  - [HyperLink](#hyperlink)
  - [Images](#images)
  - [Lists](#lists)
  - [Tables](#tables)
  - [IFrames](#iframes)
  - [HTML Entities, Symbols and Emojis](#html-entities-symbols-and-emojis)
  - [Layout Elements](#layout-elements)
  - [HTML Forms](#html-forms)
  - [Canvas](#canvashttpsdevelopermozillaorgen-usdocswebapicanvas_api)
  - [Media](#media)
  - [HTML APIs](#html-apishttpswwwgeeksforgeeksorgexplain-apis-available-in-html5)
- [References](#references)

<!-- /code_chunk_output -->


### HTML

- HTML (HyperText Markup Language) is used to create a website
- It describes the structure of Web page
- It contains series of elements
- HTML elements tell the browser how to display the content

### Editors
- Text Editor (Notepad / Notepad++)
- Visual Studio Code

### Basic Structure of HTML

```
<!DOCTYPE html> -> declaration defines that this document is an HTML5 document
<html> -> root element of an HTML page
    <head> -> contains meta information about the HTML page
        <title>Page Title</title> -> specifies a title for the HTML page (which is shown in the browser's title bar or in the page's tab)
        <meta charset="UTF-8"> -> character set
        <meta name="keywords" content="HTML, CSS, JavaScript"> -> keywords for search engines
        <meta name="description" content="Web tutorials"> ->  description of your web page
        <meta name="author" content="Sivaram"> ->  author of a page:
        <meta http-equiv="refresh" content="30"> -> Refresh document every 30 seconds
        <meta name="viewport" content="width=device-width, initial-scale=1.0"> -> Setting the viewport to make your website look good on all devices
    </head>
<body>
    <!--  the document's body, and is a container for all the visible contents, such as headings, paragraphs, images, hyperlinks, tables, lists, etc.
 -->
   <!-- This is comment -->

</body>
</html>

```
### Extension
```
.html or .htm
```
### HTML Elements && Attributes
```
A HTML element is defined by start tag , content and an end tag.

<tagName>Content</tagName>

A HTML elements can have attributes, It provide additional information about elements
<img src="img.jpg">
<p><img src="smiley.gif" alt="Smiley face" style="float:right;width:42px;height:42px;">
```
### Block Level vs Inline
- A block-level element always starts on a new line and takes up the full width available
- An inline element does not start on a new line and it only takes up as much width as necessary
- The `<div>` element is a block-level and is often used as a container for other HTML elements
- The `<span>` element is an inline container used to mark up a part of a text, or a part of a document

### To View HTML Source from Browser

- Click CTRL + U in an HTML page, or right-click on the page and select "View Page Source". This will open a new tab containing the HTML source code of the page.

- Inspect an HTML Element: Right-click on an element (or a blank area), and choose "Inspect" to see what elements are made up of (you will see both the HTML and the CSS). You can also edit the HTML or CSS on-the-fly in the Elements or Styles panel that opens.

### Different Tags
#### Headings
```
<h1>Heading 1</h1>
<h2>Heading 2</h2>
<h3>Heading 3</h3>
<h4>Heading 4</h4>
<h5>Heading 5</h5>
<h6>Heading 6</h6>
```
#### Paragraph
```
<p>This is a paragraph.</p>
<p>This is another paragraph.</p>
```
#### Styles
```
The HTML style attribute is used to add styles to an element, such as color, font, size, and more.
<p>I am normal</p>
<p style="color:red;">I am red</p>
<p style="color:blue;">I am blue</p>
<p style="font-size:50px;">I am big</p>

```
#### Formatting
```
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

#### Quotation Tags
```
<p>WWF's goal is to: <q>Build a future where people live in harmony with nature.</q></p>
<p>The <abbr title="World Health Organization">WHO</abbr> was founded in 1948.</p>
<address>
Written by John Doe.<br>
Visit us at:<br>
Example.com<br>
Box 564, Disneyland<br>
USA
</address>
<bdo dir="rtl">This text will be written from right to left</bdo>
<marquee>...</marquee>
```

#### Colors
```
HTML colors are specified with predefined color names, or with RGB, HEX, HSL, RGBA, or HSLA values.
<h1 style="background-color:tomoto;">...</h1>
<h1 style="background-color:rgb(255, 99, 71);">...</h1>
<h1 style="background-color:#ff6347;">...</h1>
<h1 style="background-color:hsl(9, 100%, 64%);">...</h1>
Ref: https://html-color-codes.info/
```

#### HyperLink
```
Allow users to click their way from page to page.

<a href="url">link text</a>
<a href="mailto:someone@example.com">Send email</a> -> Link to Email

```
| Attribute| Value or Desc |
| -------- | ------- |
| target  | _self, _blank, _parent, _top    |
| title  | specify anything   |
| id  | used for bookmark in same page|

#### Images
```
<img src="pic_trulli.jpg" alt="Italian Trulli">
Image Formats: ICO, JPEG, JPG, PNG, SVG

```
| Attribute| Value or Desc |
| -------- | ------- |
| alt  | Alternative text if img fails to load   |
| width  | width of img   |
| height  | height of img |

#### Lists
<b>UnOrdered Lists:</b>

```
<ul>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ul>
```

<b>Ordered Lists:</b>

```
<ol>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol>
```
<b>Description Lists:</b>
```
<dl>
  <dt>Coffee</dt>
  <dd>- black hot drink</dd>
  <dt>Milk</dt>
  <dd>- white cold drink</dd>
</dl>
```

#### Tables

- HTML tables allow web developers to arrange data into rows and columns.
```
<table>
  <tr>
    <th>....</th>  -> Table Header
    <th>....</th>
  </tr>
  <tr> -> Table Row
    <td>....</td> -> Table Data
    <td>....</td>
  </tr>
</table>
```

| Attribute| Desc |
| -------- | ------- |
| colspan  | represents the number of columns to span.   |
| rowspan   | represents the number of rows to span.   |
#### IFrames
```
An inline frame is used to embed another document within the current HTML document.

<iframe src="url" title="description"></iframe>

<iframe src="demo_iframe.htm" name="iframe_a" title="Iframe Example"></iframe>

<p><a href="https://www.w3schools.com" target="iframe_a">W3Schools.com</a></p>

```

#### HTML Entities, Symbols and Emojis
```
<h2>The copyright sign: &copy;</h2>
<p>I will display &#128640;</p>
<h2>The trademark symbol: &trade;</h2>
```

- [Symbols](https://www.toptal.com/designers/htmlarrows/symbols/)
- [Entities](https://www.freeformatter.com/html-entities.html)
- [Emojis](https://dev.to/rodrigoodhin/list-of-emojis-hex-codes-35ma)


#### Layout Elements
- HTML has several semantic elements that define the different parts of a web page

  ![Semantic Elements](img_sem_elements.gif)

- Responsive Web Design ([RWD](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_responsive_media_query3)) is about creating web pages that look good on all devices!  (desktops, tablets, and phones)
- Layout Techniques:
    - CSS framework: [Bootstrap](https://getbootstrap.com/), [Tailwandcss](https://tailwindcss.com/) ...
    - CSS float property
    - [CSS flexbox](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_flexible_box_layout/Basic_concepts_of_flexbox)
    - [CSS grid](https://css-tricks.com/snippets/css/complete-guide-grid/)

#### HTML Forms
-  A Form is used to collect user input. The user input is most often sent to a server for processing.
```
<form>
  ...elements here: <input>, <label>, <select>, <textarea>, <button>, <output>...
</form>

input types: checkbox,color, date, datetime-local, email,file, hidden, image, month,number, password,radio,range,reset,search,submit,tel,text,time,url,week
<input type="text"> -> Default
input Attributes: value, readonly disabled, size, maxlength, min, max, pattern , placeholder , required , step , autofocus 

```
| Attribute| Value or Desc|
| -------- | ------- |
| action  | represents the number of columns to span.   |
| target   | specifies where to display the response that is received after submitting the form  |
| method   | HTTP method to be used when submitting the form data (GET, POST, PUT, DELETE...)   |

#### [Canvas](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API)

- It is used to draw graphics on a web page.
```
<canvas id="myCanvas" width="200" height="100" style="border:1px solid #000000;">
</canvas>
```

#### Media

- Multimedia on the web is sound, music, videos, movies, and animations.
- Audio Formats: MP3, Ogg, WAV, MP4, ...
- Video Formats: MP4, WebM, Ogg, AVI, MPEG, WMV,...
```
Video:
<video width="320" height="240" controls muted autoplay>
  <source src="movie.mp4" type="video/mp4">
  <source src="movie.ogg" type="video/ogg">
</video>

Audio:
<audio controls>
  <source src="horse.ogg" type="audio/ogg">
  <source src="horse.mp3" type="audio/mpeg">
</audio>

YouTube Video:
<iframe width="420" height="315"
src="https://www.youtube.com/embed/tgbNymZ7vqY">
</iframe>
```

#### [HTML APIs](https://www.geeksforgeeks.org/explain-apis-available-in-html5/)

### References
- https://www.dcpehvpm.org/E-Content/BCA/BCA-II/Web%20Technology/the-complete-reference-html-css-fifth-edition.pdf
- https://www.geeksforgeeks.org/html/
- https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Document_and_website_structure#planning_a_simple_website
- https://developer.mozilla.org/en-US/docs/Learn/Accessibility/HTML
- https://htmlcolorcodes.com/color-picker/
- https://www.geeksforgeeks.org/top-10-projects-for-beginners-to-practice-html-and-css-skills/
- https://tiiny.host/free-static-website-hosting/
- https://render.com/docs/static-sites
- https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site

***
Thank you by ***Sivaram.N***

[sivaram.github.io](sivaram.github.io)
***
