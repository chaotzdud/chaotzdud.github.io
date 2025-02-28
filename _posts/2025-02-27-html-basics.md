---
title: HTML Basics 
date: 2025-02-27
categories: [HTML]
tags: [HTML, Web, Internet]
---

# **HTML Basics**

This is a resume from [W3S HTML Tutorial](https://www.w3schools.com/html).

---

## **1. HTML Tables**

A table in HTML consists of table cells inside rows and columns

> **Code Example:**
> 
> ```html
> <table> 
>   <tr> <!-- Table Row 1 -->
>     <th>Name</th> <!-- Table Header -->
>     <th>Age</th> <!-- Table Header -->
>     <th>Contact</th> <!-- Table Header -->
>   </tr>
> 
>   <tr> <!-- Table Row 2 -->
>     <td>Dudz</td> <!-- Table Data-->
>     <td>20</td> <!-- Table Data-->
>     <td>github.com/chaotzdud</td> <!-- Table Data-->
>   </tr>
> </table>
> ```
> 
> **Output:**
> 
> | Name | Age | Contact              |
> | ---- | --- | -------------------- |
> | Dudz | 20  | github.com/chaotzdud |
> 
> ---

## **2. HTML Lists**

### **2.1. Unordered Lists**

> **Code Example**
> ```html
> <ul>
>  <li>Coffee</li>
>  <li>Tea</li>
>  <li>Milk</li>
> </ul>
> ```
>
> **Output**
> * Coffee
> * Tea
> * Milk

### **2.2. Ordered Lists**

> **Code Example**
> ```html
> <ol>
>  <li>Coffee</li>
>  <li>Tea</li>
>  <li>Milk</li>
> </ol>
> ```
>
> **Output**
> 1. Coffee
> 2. Tea
> 3. Milk

### **2.3. Description Lists**

> **Code Example**
> 
> ```html
> <dl>
> <dt>Coffee</dt>
> <dd>- black hot drink</dd>
> <dt>Milk</dt>
> <dd>- white cold drink</dd>
> </dl>
> ```
>
> **Output**
> 
> Coffee
> - black hot drink
> 
> Milk
> - white cold drink

---

## **3. The Head Element**

The HTML <head> element is a container for the following elements: 
`<title>`, `<style>`, `<meta>`, `<link>`, `<script>`, and `<base>`.

### **3.1. The HTML \<title\> Element**

- Defines a title in the browser toolbar
- Provides a title for the page when it is added to favorites
- Displays a title for the page in search engine-results

```html
<head>
  <title>Page Title</title>
</head>
```

### **3.2. The HTML \<style\> Element**

The \<style\> element is used to define style information for a single HTML page:

```html
<style>
  body {background-color: powderblue;}
  h1 {color: red;}
  p {color: blue;}
</style>
```

### **3.3. The HTML \<link\> Element**

The \<link\> element defines the relationship between the current document and an external resource.

```html
<!-- External CSS Link Example -->
<link rel="stylesheet" href="style.css">
```

### **3.4. The HTML \<meta\> Element**

The \<meta\> element is typically used to specify the character set, page description, keywords, author of the document, and viewport settings.

The metadata will not be displayed on the page, but is used by browsers (how to display content or reload page), by search engines (keywords), and other web services.

```html
<head>
  <meta charset="UTF-8"> 
  <meta name="description" content="Free Web tutorials">
  <meta name="keywords" content="HTML, CSS, JavaScript">
  <meta name="author" content="John Doe">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
</head>
```

### **3.5. The HTML `<script>` Element**

The `<script>` element is used to define client-side JavaScripts.

```html
<script>
function myFunction() {
  document.getElementById("demo").innerHTML = "Hello JavaScript!";
}
</script>
```

### **3.6. The HTML `<base>` Element**

he `<base>` element specifies the base URL and/or target for all relative URLs in a page.

The `<base>` tag must have either an href or a target attribute present, or both.

```html
<head>
  <base href="https://www.w3schools.com/" target="_blank">
</head>

<body>
  <img src="images/stickman.gif" width="24" height="39" alt="Stickman">
  <a href="tags/tag_base.asp">HTML base Tag</a>
</body>
```

---

## **4. HTML Layout Elements and Techniques**

### **4.1. HTML Layout Elements**

![alt text](https://www.w3schools.com/html/img_sem_elements.gif)

- `<header>` - Defines a header for a document or a section
- `<nav>` - Defines a set of navigation links
- `<section>` - Defines a section in a document
- `<article>` - Defines independent, self-contained content
- `<aside>` - Defines content aside from the content (like a sidebar)
- `<footer>` - Defines a footer for a document or a section
- `<details>` - Defines additional details that the user can open and close on demand
- `<summary>` - Defines a heading for the `<details>` element

### **4.2. HTML Layout Techniques**

There are four different techniques to create multicolumn layouts. Each technique has its pros and cons:
- CSS framework
- CSS float property
- CSS flexbox
- CSS grid

---

## **5. HTML Computer Code Elements**

- The `<kbd>` element defines keyboard input
- The `<samp>` element defines sample output from a computer program
- The `<code>` element defines a piece of computer code
- The `<var>` element defines a variable in programming or in a mathematical expression
- The `<pre>` element defines preformatted text

---

## **6. HTML Semantic Elements**

> Semantic elements = elements with a meaning.

In HTML there are several semantic elements that can be used to define different parts of a web page:  

![alt text](https://www.w3schools.com/html/img_sem_elements.gif)

- `<article>`
- `<aside>`
- `<details>`
- `<figcaption>`
- `<figure>`
- `<footer>`
- `<header>`
- `<main>`
- `<mark>`
- `<nav>`
- `<section>`
- `<summary>`
- `<time>`

### **6.1. HTML `<section>` Element**

The `<section>` element defines a section in a document.

According to W3C's HTML documentation: "A section is a thematic grouping of content, typically with a heading."

Examples of where a `<section>` element can be used:
- Chapters
- Introduction
- News items
- Contact information

```html
<section>
<h1>WWF</h1>
<p>The World Wide Fund for Nature (WWF) is an international organization working on issues regarding the conservation, research and restoration of the environment, formerly named the World Wildlife Fund. WWF was founded in 1961.</p>
</section>

<section>
<h1>WWF's Panda symbol</h1>
<p>The Panda has become the symbol of WWF. The well-known panda logo of WWF originated from a panda named Chi Chi that was transferred from the Beijing Zoo to the London Zoo in the same year of the establishment of WWF.</p>
</section>
```

### **6.2. HTML `<article>` Element**

The `<article>` element specifies independent, self-contained content.

An article should make sense on its own, and it should be possible to distribute it independently from the rest of the web site.

Examples of where a `<article>` element can be used:
- Forum posts
- Blog posts
- User comments
- Product cards
- Newspaper article

```html
<article>
<h2>Google Chrome</h2>
<p>Google Chrome is a web browser developed by Google, released in 2008. Chrome is the world's most popular web browser today!</p>
</article>

<article>
<h2>Mozilla Firefox</h2>
<p>Mozilla Firefox is an open-source web browser developed by Mozilla. Firefox has been the second most popular web browser since January, 2018.</p>
</article>

<article>
<h2>Microsoft Edge</h2>
<p>Microsoft Edge is a web browser developed by Microsoft, released in 2015. Microsoft Edge replaced Internet Explorer.</p>
</article>
```

### **6.3. HTML `<header>` Element**

The `<header>` element represents a container for introductory content or a set of navigational links.

A `<header>` element typically contains:
- one or more heading elements (`<h1>` - `<h6>`)
- ogo or icon
- authorship information

Examples of where a `<header>` element can be used:
- Forum posts
- Blog posts
- User comments
- Product cards
- Newspaper header

```html
<article>
  <header>
    <h1>What Does WWF Do?</h1>
    <p>WWF's mission:</p>
  </header>
  <p>WWF's mission is to stop the degradation of our planet's natural environment,
  and build a future in which humans live in harmony with nature.</p>
</article>
```

### **6.4. HTML `<footer>` Element**

The `<footer>` element defines a footer for a document or section.

A `<footer>` element typically contains:

- authorship information
- copyright information
- contact information
- sitemap
- back to top links
- related documents
- You can have several `<footer>` elements in one document.

```html
<footer>
  <p>Author: Hege Refsnes</p>
  <p><a href="mailto:hege@example.com">hege@example.com</a></p>
</footer
```

### **6.5. HTML `<nav>` Element**

The `<nav>` element defines a set of navigation links.

> Notice that NOT all links of a document should be inside a `<nav>` element. The `<nav>` element is intended only for major blocks of navigation links.
> Browsers, such as screen readers for disabled users, can use this element to determine whether to omit the initial rendering of this content.

```html
<nav>
  <a href="/html/">HTML</a> |
  <a href="/css/">CSS</a> |
  <a href="/js/">JavaScript</a> |
  <a href="/jquery/">jQuery</a>
</nav>
```

### **6.6. HTML `<aside>` Element**

The <aside> element defines some content aside from the content it is placed in (like a sidebar).

The <aside> content should be indirectly related to the surrounding content.

```html
<p>My family and I visited The Epcot center this summer. The weather was nice, and Epcot was amazing! I had a great summer together with my family!</p>

<aside>
<h4>Epcot Center</h4>
<p>Epcot is a theme park at Walt Disney World Resort featuring exciting attractions, international pavilions, award-winning fireworks and seasonal special events.</p>
</aside>
```

### **6.7. HTML `<figure>` and `<figcaption>` Elements**

The `<figure>` tag specifies self-contained content, like illustrations, diagrams, photos, code listings, etc.

The `<figcaption>` tag defines a caption for a `<figure>` element. The `<figcaption>` element can be placed as the first or as the last child of a `<figure>` element.

The `<img>` element defines the actual image/illustration. 

```html
<figure>
  <img src="pic_trulli.jpg" alt="Trulli">
  <figcaption>Fig1. - Trulli, Puglia, Italy.</figcaption>
</figure>
```

## **7. HTML Character Entities**

| Result       | Description           | Name      | Number    |
| ------------ | --------------------- | --------- | --------- |
| non-breaking | space                 | `&nbsp;`  | `&#160;`  |
| <            | less than             | `&lt;`    | `&#60;`   |
| >            | greater than          | `&gt;`    | `&#62;`   |
| &            | ampersand             | `&amp;`   | `&#38;`   |
| "            | double quotation mark | `&quot;`  | `&#34;`   |
| '            | single quotation mark | `&apos;`  | `&#39;`   |
| ¢            | cent                  | `&cent;`  | `&#162;`  |
| £            | pound                 | `&pound;` | `&#163;`  |
| ¥            | yen                   | `&yen;`   | `&#165;`  |
| €            | euro                  | `&euro;`  | `&#8364;` |
| ©            | copyright             | `&copy;`  | `&#169;`  |
| ®            | trademark             | `&reg;`   | `&#174;`  |

## **8. HTML Symbols**

| Char | Number    | Entity     | Description          |
| ---- | --------- | ---------- | -------------------- |
| ∀    | `&#8704;` | `&forall;` | For all              |
| ∂    | `&#8706;` | `&part;`   | Partial differential |
| ∃    | `&#8707;` | `&exist;`  | There exists         |
| ∅    | `&#8709;` | `&empty;`  | Empty sets           |
| ∇    | `&#8711;` | `&nabla;`  | Nabla                |
| ∈    | `&#8712;` | `&isin;`   | Element of           |
| ∉    | `&#8713;` | `&notin;`  | Not an element of    |
| ∋    | `&#8715;` | `&ni;`     | Contains as member   |
| ∏    | `&#8719;` | `&prod;`   | N-ary product        |
| ∑    | `&#8721;` | `&sum;`    | N-ary summatio       |

## **9. HTML Encoding (Character Sets)**

![https://www.w3schools.com/images/unicode_web.jpg](https://www.w3schools.com/images/unicode_web.jpg)

### **9.1. The ASCII Character Set**

ASCII was the first character encoding standard for the web. It defined 128 different characters that could be used on the internet:
- English letters (A-Z)
- Numbers (0-9)
- Special characters like ! $ + - ( ) @ < >.

### **9.2. The ANSI Character Set**

ANSI (Windows-1252) was the original Windows character set:
- Identical to ASCII for the first 127 characters
- Special characters from 128 to 159
- Identical to UTF-8 from 160 to 255

```html
<meta charset="Windows-1252">
```

### **9.3. The ISO-8859-1 Character Set**

ISO-8859-1 was the default character set for HTML 4. This character set supported 256 different character codes. HTML 4 also supported UTF-8.
- Identical to ASCII for the first 127 characters
- Does not use the characters from 128 to 159
- Identical to ANSI and UTF-8 from 160 to 255

> **HTML 4 Example**
> ```html
> <meta http-equiv="Content-Type" content="text/html;charset=ISO-8859-1">
> ```
> 
> **HTML 5 Example**
> ```html
> <meta charset="ISO-8859-1">
> ```

### **9.4. The UTF-8 Character Set**

- is identical to ASCII for the values from 0 to 127
- Does not use the characters from 128 to 159
- Identical to ANSI and 8859-1 from 160 to 255
- Continues from the value 256 to 10 000 characters

```html
<meta charset="UTF-8">
```

## **10. HTML Uniform Resource Locators**

A URL is another word for a web address.

A URL can be composed of words (e.g. w3schools.com), or an Internet Protocol (IP) address (e.g. 192.68.20.50).

Most people enter the name when surfing, because names are easier to remember than numbers.

### **10.1. URL  Uniform Resource Locator**

Web browsers request pages from web servers by using a URL.

A Uniform Resource Locator (URL) is used to address a document (or other data) on the web.

A web address like https://www.w3schools.com/html/default.asp follows these syntax rules:

```
scheme://prefix.domain:port/path/filename
```

Explanation:
- **scheme** - defines the **type** of Internet service (most common is **http** or **https**)
- **prefix** - defines a domain **prefix** (default for http is **www**)
- **domain** - defines the Internet **domain name** (like w3schools.com)
- **port** - defines the **port number** at the host (default for http is **80**)
- **path** - defines a **path** at the server (If omitted: the root directory of the site)
- **filename** - defines the name of a document or **resource**